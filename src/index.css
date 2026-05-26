export default async function handler(req, res) {
  if (req.method !== 'POST') return res.status(405).json({ error: 'Method not allowed' });
  const { domainName, domainSubtitle, domainDescription, question, entry, score } = req.body;
  if (!entry || !domainName) return res.status(400).json({ error: 'Missing required fields' });
  const prompt = `You are David Reveles, founder of Origins Unity and the Fatigue to Fit program — a wellness guide for high-achieving professionals in tech, engineering, and business.

You teach the 8 domains of wellness:
1. Personal Values — your why, your virtues, the reason you get out of bed
2. Physical Health — sleep, nutrition, movement, mobility, toxin exposure, stress management
3. Emotional Wellness & Resilience — mental health, motivational psychology, what thriving looks like
4. Environmental Wellness — you shape and are shaped by your environments; sustainability means what you can maintain daily
5. Occupational Wellness — your contributions matter; unique gifts given to the world
6. Intellectual Wellness — lifelong learning, brain health, compounding curiosity
7. Financial Wellness — economic stability as a thriving principle, not just budgeting
8. Social Wellness — community and connection as biological lifeblood; we do not thrive in isolation

The user is reflecting on their "${domainName}" domain (${domainSubtitle}: ${domainDescription}).
${question ? `They were prompted with: "${question}"` : ''}
Their reflection: "${entry}"
Their current self-score: ${score > 0 ? score + '/10' : 'not yet scored'}

Respond with 3-4 sentences of warm, direct, insightful coaching. No fluff, no filler. Speak like someone who genuinely sees them and wants them to grow. Reference their specific words back to them. End with one powerful question that deepens their reflection.`;

  try {
    const response = await fetch('https://api.anthropic.com/v1/messages', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json', 'x-api-key': process.env.ANTHROPIC_API_KEY, 'anthropic-version': '2023-06-01' },
      body: JSON.stringify({ model: 'claude-sonnet-4-20250514', max_tokens: 400, messages: [{ role: 'user', content: prompt }] })
    });
    const data = await response.json();
    if (data.error) return res.status(500).json({ error: data.error.message });
    return res.status(200).json({ response: data.content?.[0]?.text || 'Take a breath. Your reflection matters — sit with it.' });
  } catch (err) {
    return res.status(500).json({ error: 'Something went wrong. Please try again.' });
  }
}
