import { useState, useEffect } from "react";

// ─── Domain Data ───────────────────────────────────────────────────────────────
const DOMAINS = [
  {
    id: "values",
    name: "Personal Values",
    subtitle: "Your Why",
    icon: "◈",
    color: "#C4782A",
    description: "Your virtues, your compass, the reason you get out of bed. Everything else roots here.",
    questions: [
      { text: "Do I have a clear sense of meaning and purpose in my life?", type: "yesno" },
      { text: "Do I have values and beliefs that I base my life around?", type: "yesno" },
      { text: "Are my daily actions aligned with my deepest values?", type: "yesno" },
      { text: "Do I have a feeling of inner peace?", type: "yesno" },
      { text: "Am I able to forgive myself and others when needed?", type: "yesno" },
      { text: "Do I know my 'why' — the core reason I do what I do?", type: "yesno" },
      { text: "When I face a hard decision, do I have a values-based compass to guide me?", type: "yesno" },
      { text: "What value do I most need to honor more fully right now?", type: "reflect" },
      { text: "Is there a gap between who I say I am and how I actually show up?", type: "reflect" },
      { text: "What would I do differently if I lived more aligned with my values?", type: "reflect" }
    ]
  },
  {
    id: "physical",
    name: "Physical Health",
    subtitle: "The Full Ecosystem",
    icon: "⬡",
    color: "#7B9E4E",
    description: "Sleep, nutrition, movement, mobility, toxin exposure, acute stress management.",
    questions: [
      { text: "Do I eat a balanced, nutritional diet that genuinely nourishes me?", type: "yesno" },
      { text: "Do I exercise or move my body at least three times a week?", type: "yesno" },
      { text: "Am I getting consistent, quality sleep most nights?", type: "yesno" },
      { text: "Am I generally free from chronic illness or unmanaged health issues?", type: "yesno" },
      { text: "Am I at a healthy weight and energy level for my body?", type: "yesno" },
      { text: "Do I manage acute stress in healthy, constructive ways?", type: "yesno" },
      { text: "Am I mindful of my exposure to toxins — substances, environments, inputs?", type: "yesno" },
      { text: "Do I use alcohol or other substances safely and intentionally?", type: "yesno" },
      { text: "Where is my body asking for more attention right now?", type: "reflect" },
      { text: "Am I fueling my body or truly nourishing it — what's the difference for me?", type: "reflect" }
    ]
  },
  {
    id: "emotional",
    name: "Emotional Wellness",
    subtitle: "Inner Resilience",
    icon: "◎",
    color: "#5B8FA8",
    description: "Mental health, resilience, motivational psychology — what thriving actually looks like for you.",
    questions: [
      { text: "Am I able to express and communicate my feelings openly?", type: "yesno" },
      { text: "Do I have a healthy level of control over my emotional responses?", type: "yesno" },
      { text: "Am I able to adapt to change without being destabilized?", type: "yesno" },
      { text: "Am I emotionally stable the majority of the time?", type: "yesno" },
      { text: "Do I have healthy ways to process difficult emotions?", type: "yesno" },
      { text: "Am I able to ask for help when I'm struggling emotionally?", type: "yesno" },
      { text: "Do I practice self-compassion rather than harsh self-criticism?", type: "yesno" },
      { text: "What emotion has shown up most in my life this week?", type: "reflect" },
      { text: "Where am I thriving emotionally — and where am I just surviving?", type: "reflect" },
      { text: "What does my inner dialogue sound like when no one else can hear it?", type: "reflect" }
    ]
  },
  {
    id: "environmental",
    name: "Environmental Wellness",
    subtitle: "You Shape & Are Shaped",
    icon: "◉",
    color: "#8A7B5C",
    description: "You are a product of your environments — and your environments are a product of you.",
    questions: [
      { text: "Does my primary environment — home, work, daily spaces — energize me?", type: "yesno" },
      { text: "Am I intentional about the environments I place myself in?", type: "yesno" },
      { text: "Do I take care of my physical surroundings in a way I can sustain?", type: "yesno" },
      { text: "Am I aware of how my environments influence my mood and behavior?", type: "yesno" },
      { text: "Do I take steps to reduce my exposure to toxic environments — digital, social, physical?", type: "yesno" },
      { text: "Do I make choices that support environmental sustainability in my daily life?", type: "yesno" },
      { text: "Am I contributing positively to the environments I inhabit?", type: "yesno" },
      { text: "What environment am I in most often — and is it helping or hurting me?", type: "reflect" },
      { text: "Where am I being influenced without fully realizing it?", type: "reflect" },
      { text: "What is one change to my environment that would most improve my wellbeing?", type: "reflect" }
    ]
  },
  {
    id: "occupational",
    name: "Occupational Wellness",
    subtitle: "Your Gifts Matter",
    icon: "◇",
    color: "#A8704E",
    description: "Your contributions have impact. Find meaning — in your work, your vocation, your service.",
    questions: [
      { text: "Do I find meaning or satisfaction in the work I do?", type: "yesno" },
      { text: "Do I communicate well with colleagues, clients, or collaborators?", type: "yesno" },
      { text: "Have I set realistic goals for my career or vocational path?", type: "yesno" },
      { text: "Am I making progress toward those goals?", type: "yesno" },
      { text: "Do I feel that my unique gifts and skills are being used?", type: "yesno" },
      { text: "Does my work align with my personal values?", type: "yesno" },
      { text: "Do I have a healthy separation between work and personal life?", type: "yesno" },
      { text: "What tasks at work or in my vocation do I genuinely enjoy?", type: "reflect" },
      { text: "What tasks drain me — and what does that tell me about my direction?", type: "reflect" },
      { text: "If I could contribute one thing to the world through my work, what would it be?", type: "reflect" }
    ]
  },
  {
    id: "intellectual",
    name: "Intellectual Wellness",
    subtitle: "Lifelong Growth",
    icon: "△",
    color: "#6B7FA8",
    description: "Stimulate, learn, grow. Brain health compounds — richer life, deeper connections, longer thriving.",
    questions: [
      { text: "Do I strive to learn new things and exercise my mind regularly?", type: "yesno" },
      { text: "Do I engage in mentally stimulating activities — reading, problem-solving, creating?", type: "yesno" },
      { text: "Am I actively developing new skills, personally or professionally?", type: "yesno" },
      { text: "Do I spend intentional time on personal or professional development?", type: "yesno" },
      { text: "Do I approach life with curiosity rather than assumption?", type: "yesno" },
      { text: "Do I seek out perspectives different from my own?", type: "yesno" },
      { text: "Am I investing in my brain health the same way I invest in my physical health?", type: "yesno" },
      { text: "What am I learning right now that genuinely excites me?", type: "reflect" },
      { text: "When did I last seriously challenge a belief I've held for a long time?", type: "reflect" },
      { text: "What am I curious about that I haven't given myself permission to explore yet?", type: "reflect" }
    ]
  },
  {
    id: "financial",
    name: "Financial Wellness",
    subtitle: "Economic Integrity",
    icon: "▽",
    color: "#5C8A6B",
    description: "Economic stability is a thriving principle. Know the inner workings. Sustain yourself with integrity.",
    questions: [
      { text: "Do I have a budget and am I generally able to save money?", type: "yesno" },
      { text: "Does my financial behavior reflect my values and beliefs about money?", type: "yesno" },
      { text: "Am I using my money wisely and intentionally?", type: "yesno" },
      { text: "Do I have financial goals and a plan for my future?", type: "yesno" },
      { text: "Am I financially prepared for unexpected expenses or emergencies?", type: "yesno" },
      { text: "Do I understand the economic impact of my choices and habits?", type: "yesno" },
      { text: "Am I free from financial stress the majority of the time?", type: "yesno" },
      { text: "Where do I feel financially empowered — and where does anxiety live?", type: "reflect" },
      { text: "What does true financial freedom mean to me beyond a dollar amount?", type: "reflect" },
      { text: "Is my financial life currently supporting or undermining my overall wellness?", type: "reflect" }
    ]
  },
  {
    id: "social",
    name: "Social Wellness",
    subtitle: "The Lifeblood",
    icon: "⬟",
    color: "#9A5B7A",
    description: "Community and connection are not optional. You will not thrive in isolation — ever.",
    questions: [
      { text: "Do I have people in my life that I genuinely trust?", type: "yesno" },
      { text: "Can I resolve conflicts effectively in my relationships?", type: "yesno" },
      { text: "Am I perceptive of other people's feelings and needs?", type: "yesno" },
      { text: "Do I communicate well and authentically with others?", type: "yesno" },
      { text: "Am I able to set healthy boundaries in my relationships?", type: "yesno" },
      { text: "Do I have a sense of belonging — to a community, a group, a cause?", type: "yesno" },
      { text: "Am I investing in my relationships, not just maintaining them?", type: "yesno" },
      { text: "Who in my life genuinely fills my cup — and am I protecting that relationship?", type: "reflect" },
      { text: "Where do I feel most deeply seen, known, and belonging?", type: "reflect" },
      { text: "Is loneliness present in my life in a way I haven't fully acknowledged?", type: "reflect" }
    ]
  }
];

const STORAGE_KEYS = {
  scores: "ou_scores_v1",
  journal: "ou_journal_v1",
  goals: "ou_goals_v1",
  answers: "ou_answers_v1",
  name: "ou_user_name"
};

function store(key, value) {
  try { localStorage.setItem(key, JSON.stringify(value)); } catch {}
}
function retrieve(key, fallback) {
  try { const v = localStorage.getItem(key); return v ? JSON.parse(v) : fallback; }
  catch { return fallback; }
}

// ─── Radial Score Ring ──────────────────────────────────────────────────────────
function ScoreRing({ score, color, size = 72 }) {
  const r = size / 2 - 7;
  const circ = 2 * Math.PI * r;
  const filled = score > 0 ? (score / 10) * circ : 0;
  return (
    <svg width={size} height={size} style={{ transform: "rotate(-90deg)", flexShrink: 0 }}>
      <circle cx={size/2} cy={size/2} r={r} fill="none" stroke="rgba(255,255,255,0.07)" strokeWidth="5" />
      <circle cx={size/2} cy={size/2} r={r} fill="none" stroke={color} strokeWidth="5"
        strokeDasharray={`${filled} ${circ}`} strokeLinecap="round"
        style={{ transition: "stroke-dasharray 0.9s cubic-bezier(.4,0,.2,1)" }} />
      <text x={size/2} y={size/2} textAnchor="middle" dominantBaseline="central"
        style={{
          transform: `rotate(90deg)`, transformOrigin: `${size/2}px ${size/2}px`,
          fill: score > 0 ? color : "rgba(255,255,255,0.25)",
          fontSize: score > 0 ? "16px" : "11px",
          fontFamily: "'Cormorant Garamond', Georgia, serif",
          fontWeight: "700"
        }}>
        {score > 0 ? score : "—"}
      </text>
    </svg>
  );
}

// ─── Domain Card ───────────────────────────────────────────────────────────────
function DomainCard({ domain, score, onClick, index }) {
  const [hover, setHover] = useState(false);
  return (
    <div onClick={onClick} onMouseEnter={() => setHover(true)} onMouseLeave={() => setHover(false)}
      style={{
        background: hover ? "rgba(255,255,255,0.06)" : "rgba(255,255,255,0.03)",
        border: `1px solid ${hover ? domain.color + "44" : "rgba(255,255,255,0.07)"}`,
        borderRadius: "20px", padding: "22px", cursor: "pointer",
        transition: "all 0.3s ease", transform: hover ? "translateY(-3px)" : "none",
        position: "relative", overflow: "hidden"
      }}>
      <div style={{ position: "absolute", top: 0, left: 0, right: 0, height: "3px", background: `linear-gradient(90deg, ${domain.color}, transparent)`, opacity: score > 0 ? 1 : 0.25 }} />
      <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: "14px" }}>
        <div style={{ flex: 1, paddingRight: "12px" }}>
          <div style={{ fontSize: "24px", color: domain.color, marginBottom: "6px", lineHeight: 1 }}>{domain.icon}</div>
          <div style={{ fontSize: "15px", fontWeight: "600", color: "#F5ECD7", fontFamily: "'Cormorant Garamond', serif", letterSpacing: "0.02em" }}>{domain.name}</div>
          <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.45)", marginTop: "2px", fontStyle: "italic" }}>{domain.subtitle}</div>
        </div>
        <ScoreRing score={score} color={domain.color} size={64} />
      </div>
      <div style={{ fontSize: "12.5px", color: "rgba(245,236,215,0.55)", lineHeight: "1.55" }}>{domain.description}</div>
      <div style={{ marginTop: "14px", fontSize: "11px", color: domain.color, opacity: hover ? 1 : 0, transition: "opacity 0.2s", fontWeight: "500", letterSpacing: "0.05em" }}>
        OPEN DOMAIN →
      </div>
    </div>
  );
}

// ─── Modal ─────────────────────────────────────────────────────────────────────
function DomainModal({ domain, score, onScore, onClose, journal, onJournal, goals, onGoals, answers, onAnswers }) {
  const [localScore, setLocalScore] = useState(score);
  const [tab, setTab] = useState("assess");
  const [entry, setEntry] = useState("");
  const [selectedQ, setSelectedQ] = useState(null);
  const [aiResponse, setAiResponse] = useState("");
  const [loading, setLoading] = useState(false);
  const [newGoal, setNewGoal] = useState("");
  const [domainGoals, setDomainGoals] = useState(goals[domain.id] || []);
  const [domainJournal, setDomainJournal] = useState(journal[domain.id] || []);
  const [domainAnswers, setDomainAnswers] = useState(answers[domain.id] || {});

  const yesnoQs = domain.questions.filter(q => q.type === "yesno");
  const reflectQs = domain.questions.filter(q => q.type === "reflect");

  const handleAnswer = (qText, answer) => {
    const updated = { ...domainAnswers, [qText]: answer };
    setDomainAnswers(updated);
    onAnswers(domain.id, updated);
    // Auto-calculate score from yes/no answers
    const yesCount = Object.entries(updated).filter(([k, v]) => {
      const q = yesnoQs.find(q => q.text === k);
      return q && v === "yes";
    }).length;
    const answered = yesnoQs.filter(q => updated[q.text]).length;
    if (answered >= 3) {
      const autoScore = Math.round((yesCount / yesnoQs.length) * 10);
      const clamped = Math.max(1, autoScore);
      setLocalScore(clamped);
      onScore(domain.id, clamped);
    }
  };

  const handleScore = (s) => { setLocalScore(s); onScore(domain.id, s); };

  const handleJournalSubmit = async () => {
    if (!entry.trim()) return;
    const newEntry = { text: entry, date: new Date().toLocaleDateString(), question: selectedQ };
    const updated = [newEntry, ...domainJournal].slice(0, 20);
    setDomainJournal(updated);
    onJournal(domain.id, updated);
    setLoading(true);
    setAiResponse("");
    try {
      const res = await fetch("/api/coach", {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({
          domainName: domain.name,
          domainSubtitle: domain.subtitle,
          domainDescription: domain.description,
          question: selectedQ,
          entry,
          score: localScore
        })
      });
      const data = await res.json();
      setAiResponse(data.response || "Take a breath. Your reflection matters — sit with it.");
    } catch {
      setAiResponse("Take a breath. Your reflection matters — sit with it.");
    }
    setLoading(false);
    setEntry("");
    setSelectedQ(null);
  };

  const handleAddGoal = () => {
    if (!newGoal.trim()) return;
    const updated = [{ text: newGoal, done: false, date: new Date().toLocaleDateString() }, ...domainGoals];
    setDomainGoals(updated);
    onGoals(domain.id, updated);
    setNewGoal("");
  };

  const toggleGoal = (i) => {
    const updated = domainGoals.map((g, idx) => idx === i ? { ...g, done: !g.done } : g);
    setDomainGoals(updated);
    onGoals(domain.id, updated);
  };

  const removeGoal = (i) => {
    const updated = domainGoals.filter((_, idx) => idx !== i);
    setDomainGoals(updated);
    onGoals(domain.id, updated);
  };

  const answeredCount = yesnoQs.filter(q => domainAnswers[q.text]).length;
  const tabs = ["assess", "reflect", "journal", "goals"];

  const answerColors = { yes: "#7B9E4E", no: "#A85B5B", "n/a": "#6B6B6B", unsure: "#8A7B5C" };
  const answerLabels = { yes: "Yes", no: "No", "n/a": "N/A", unsure: "Unsure" };

  return (
    <div onClick={onClose} style={{
      position: "fixed", inset: 0, zIndex: 200, background: "rgba(8,6,4,0.92)",
      display: "flex", alignItems: "center", justifyContent: "center",
      padding: "16px", backdropFilter: "blur(4px)"
    }}>
      <div onClick={e => e.stopPropagation()} style={{
        background: "#141008", border: `1px solid ${domain.color}30`,
        borderRadius: "28px", width: "100%", maxWidth: "640px",
        maxHeight: "92vh", overflowY: "auto", padding: "36px",
        position: "relative", boxShadow: `0 40px 80px rgba(0,0,0,0.6), 0 0 0 1px ${domain.color}15`
      }}>
        <div style={{ position: "absolute", top: 0, left: 0, right: 0, height: "4px", background: `linear-gradient(90deg, ${domain.color}, ${domain.color}00)`, borderRadius: "28px 28px 0 0" }} />
        <button onClick={onClose} style={{
          position: "absolute", top: "18px", right: "18px",
          background: "rgba(255,255,255,0.06)", border: "none",
          color: "rgba(245,236,215,0.5)", width: "32px", height: "32px",
          borderRadius: "50%", cursor: "pointer", fontSize: "16px",
          display: "flex", alignItems: "center", justifyContent: "center"
        }}>✕</button>

        {/* Header */}
        <div style={{ display: "flex", alignItems: "center", gap: "18px", marginBottom: "28px" }}>
          <div style={{ fontSize: "40px", color: domain.color, lineHeight: 1 }}>{domain.icon}</div>
          <div style={{ flex: 1 }}>
            <h2 style={{ fontFamily: "'Cormorant Garamond', serif", fontSize: "26px", color: "#F5ECD7", fontWeight: "700", margin: 0 }}>{domain.name}</h2>
            <div style={{ fontSize: "13px", color: "rgba(245,236,215,0.45)", fontStyle: "italic", marginTop: "3px" }}>{domain.subtitle}</div>
          </div>
          <ScoreRing score={localScore} color={domain.color} size={76} />
        </div>

        {/* Manual score override */}
        <div style={{ marginBottom: "28px" }}>
          <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.12em", marginBottom: "10px" }}>
            Overall score for this domain (auto-calculates from assessment)
          </div>
          <div style={{ display: "flex", gap: "5px" }}>
            {[1,2,3,4,5,6,7,8,9,10].map(n => (
              <button key={n} onClick={() => handleScore(n)} style={{
                flex: 1, height: "38px", borderRadius: "10px", border: "none", cursor: "pointer",
                background: n <= localScore ? domain.color : "rgba(255,255,255,0.06)",
                color: n <= localScore ? "#fff" : "rgba(255,255,255,0.3)",
                fontSize: "13px", fontWeight: "600", transition: "all 0.15s"
              }}>{n}</button>
            ))}
          </div>
        </div>

        {/* Tabs */}
        <div style={{ display: "flex", gap: "4px", background: "rgba(255,255,255,0.04)", borderRadius: "14px", padding: "4px", marginBottom: "24px" }}>
          {tabs.map(t => (
            <button key={t} onClick={() => setTab(t)} style={{
              flex: 1, padding: "9px", borderRadius: "11px", border: "none", cursor: "pointer",
              background: tab === t ? domain.color + "28" : "none",
              color: tab === t ? domain.color : "rgba(245,236,215,0.4)",
              fontSize: "12px", fontWeight: "600", textTransform: "capitalize",
              transition: "all 0.2s", letterSpacing: "0.02em"
            }}>{t}</button>
          ))}
        </div>

        {/* ASSESS TAB */}
        {tab === "assess" && (
          <div>
            <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: "14px" }}>
              <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.12em" }}>
                Quick Assessment Questions
              </div>
              <div style={{ fontSize: "12px", color: domain.color, fontWeight: "600" }}>
                {answeredCount}/{yesnoQs.length} answered
              </div>
            </div>
            {yesnoQs.map((q, i) => (
              <div key={i} style={{
                padding: "14px 16px", borderRadius: "14px", marginBottom: "10px",
                background: "rgba(255,255,255,0.03)", border: "1px solid rgba(255,255,255,0.06)"
              }}>
                <div style={{ fontSize: "13.5px", color: "#F5ECD7", lineHeight: "1.55", marginBottom: "10px" }}>{q.text}</div>
                <div style={{ display: "flex", gap: "6px" }}>
                  {["yes", "no", "unsure", "n/a"].map(opt => (
                    <button key={opt} onClick={() => handleAnswer(q.text, opt)} style={{
                      flex: 1, padding: "6px 4px", borderRadius: "8px", border: "none", cursor: "pointer",
                      background: domainAnswers[q.text] === opt ? answerColors[opt] : "rgba(255,255,255,0.06)",
                      color: domainAnswers[q.text] === opt ? "#fff" : "rgba(245,236,215,0.4)",
                      fontSize: "11px", fontWeight: "600", transition: "all 0.15s",
                      letterSpacing: "0.04em"
                    }}>{answerLabels[opt]}</button>
                  ))}
                </div>
              </div>
            ))}
            {answeredCount >= 3 && (
              <div style={{
                marginTop: "16px", padding: "14px 18px",
                background: domain.color + "15", borderRadius: "12px",
                border: `1px solid ${domain.color}30`,
                fontSize: "13px", color: "rgba(245,236,215,0.8)", textAlign: "center"
              }}>
                Score auto-calculated: <strong style={{ color: domain.color }}>{localScore}/10</strong> — adjust manually above if needed, then visit <strong>Reflect</strong> to go deeper.
              </div>
            )}
          </div>
        )}

        {/* REFLECT TAB */}
        {tab === "reflect" && (
          <div>
            <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.12em", marginBottom: "12px" }}>
              Deeper Reflection Prompts
            </div>
            {reflectQs.map((q, i) => (
              <div key={i} onClick={() => { setSelectedQ(q.text); setTab("journal"); }}
                style={{
                  padding: "16px 18px", borderRadius: "14px", marginBottom: "10px",
                  background: "rgba(255,255,255,0.04)", border: `1px solid rgba(255,255,255,0.07)`,
                  cursor: "pointer", color: "#F5ECD7", fontSize: "14px", lineHeight: "1.6",
                  transition: "all 0.2s"
                }}
                onMouseEnter={e => { e.currentTarget.style.background = domain.color + "15"; e.currentTarget.style.borderColor = domain.color + "40"; }}
                onMouseLeave={e => { e.currentTarget.style.background = "rgba(255,255,255,0.04)"; e.currentTarget.style.borderColor = "rgba(255,255,255,0.07)"; }}>
                {q.text}
              </div>
            ))}
            <div style={{ textAlign: "center", marginTop: "8px", fontSize: "12px", color: "rgba(245,236,215,0.3)", fontStyle: "italic" }}>
              Tap a prompt to journal your reflection →
            </div>
          </div>
        )}

        {/* JOURNAL TAB */}
        {tab === "journal" && (
          <div>
            {selectedQ && (
              <div style={{
                padding: "12px 16px", background: domain.color + "15",
                border: `1px solid ${domain.color}30`, borderRadius: "12px",
                marginBottom: "14px", fontSize: "13px", color: domain.color,
                fontStyle: "italic", lineHeight: "1.5"
              }}>"{selectedQ}"</div>
            )}
            <textarea value={entry} onChange={e => setEntry(e.target.value)}
              placeholder="What's true for you in this domain right now..."
              style={{
                width: "100%", minHeight: "130px", background: "rgba(255,255,255,0.04)",
                border: "1px solid rgba(255,255,255,0.1)", borderRadius: "14px",
                padding: "16px", color: "#F5ECD7", fontSize: "14px", lineHeight: "1.65",
                resize: "vertical", fontFamily: "'DM Sans', sans-serif", outline: "none",
                boxSizing: "border-box"
              }}
            />
            <button onClick={handleJournalSubmit} disabled={loading || !entry.trim()} style={{
              marginTop: "10px", width: "100%", padding: "14px",
              background: entry.trim() && !loading ? domain.color : "rgba(255,255,255,0.08)",
              border: "none", borderRadius: "12px",
              color: entry.trim() && !loading ? "#fff" : "rgba(255,255,255,0.3)",
              fontSize: "14px", fontWeight: "600", cursor: entry.trim() && !loading ? "pointer" : "default",
              transition: "all 0.2s", letterSpacing: "0.03em"
            }}>
              {loading ? "Reflecting with you..." : "Submit & Receive Coaching"}
            </button>

            {aiResponse && (
              <div style={{
                marginTop: "18px", padding: "18px 20px", background: "rgba(255,255,255,0.03)",
                borderRadius: "14px", borderLeft: `3px solid ${domain.color}`,
                color: "rgba(245,236,215,0.85)", fontSize: "14px", lineHeight: "1.75", fontStyle: "italic"
              }}>
                <div style={{ fontSize: "10px", color: domain.color, textTransform: "uppercase", letterSpacing: "0.15em", marginBottom: "10px", fontStyle: "normal", fontWeight: "600" }}>David's Coaching</div>
                {aiResponse}
              </div>
            )}

            {domainJournal.length > 0 && (
              <div style={{ marginTop: "24px" }}>
                <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.35)", textTransform: "uppercase", letterSpacing: "0.12em", marginBottom: "10px" }}>Past reflections</div>
                {domainJournal.map((j, i) => (
                  <div key={i} style={{
                    padding: "12px 16px", background: "rgba(255,255,255,0.03)",
                    borderRadius: "12px", marginBottom: "8px", border: "1px solid rgba(255,255,255,0.05)"
                  }}>
                    <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.3)", marginBottom: "5px" }}>{j.date}</div>
                    <div style={{ fontSize: "13px", color: "rgba(245,236,215,0.65)", lineHeight: "1.5" }}>{j.text}</div>
                  </div>
                ))}
              </div>
            )}
          </div>
        )}

        {/* GOALS TAB */}
        {tab === "goals" && (
          <div>
            <div style={{ display: "flex", gap: "8px", marginBottom: "18px" }}>
              <input value={newGoal} onChange={e => setNewGoal(e.target.value)}
                onKeyDown={e => e.key === "Enter" && handleAddGoal()}
                placeholder="Add an action for this domain..."
                style={{
                  flex: 1, padding: "12px 16px", background: "rgba(255,255,255,0.05)",
                  border: "1px solid rgba(255,255,255,0.1)", borderRadius: "12px",
                  color: "#F5ECD7", fontSize: "13px", outline: "none", fontFamily: "'DM Sans', sans-serif"
                }}
              />
              <button onClick={handleAddGoal} style={{
                padding: "12px 18px", background: domain.color, border: "none",
                borderRadius: "12px", color: "#fff", fontWeight: "700", fontSize: "18px", cursor: "pointer"
              }}>+</button>
            </div>
            {domainGoals.length === 0 && (
              <div style={{ textAlign: "center", padding: "32px", color: "rgba(245,236,215,0.3)", fontSize: "13px", fontStyle: "italic" }}>
                No actions yet.<br />What's one step you can take in this domain?
              </div>
            )}
            {domainGoals.map((g, i) => (
              <div key={i} style={{
                display: "flex", alignItems: "center", gap: "12px",
                padding: "13px 16px", background: "rgba(255,255,255,0.04)",
                borderRadius: "12px", marginBottom: "7px", border: "1px solid rgba(255,255,255,0.05)",
                opacity: g.done ? 0.5 : 1, transition: "opacity 0.2s"
              }}>
                <div onClick={() => toggleGoal(i)} style={{
                  width: "20px", height: "20px", borderRadius: "50%", flexShrink: 0,
                  border: `2px solid ${g.done ? domain.color : "rgba(255,255,255,0.2)"}`,
                  background: g.done ? domain.color : "none", cursor: "pointer",
                  display: "flex", alignItems: "center", justifyContent: "center",
                  fontSize: "11px", color: "#fff", transition: "all 0.2s"
                }}>{g.done ? "✓" : ""}</div>
                <div style={{ flex: 1, fontSize: "13px", color: "#F5ECD7", textDecoration: g.done ? "line-through" : "none", cursor: "pointer" }} onClick={() => toggleGoal(i)}>{g.text}</div>
                <div style={{ fontSize: "11px", color: "rgba(245,236,215,0.25)", flexShrink: 0 }}>{g.date}</div>
                <button onClick={() => removeGoal(i)} style={{ background: "none", border: "none", color: "rgba(245,236,215,0.2)", cursor: "pointer", fontSize: "14px", padding: "0 4px" }}>×</button>
              </div>
            ))}
          </div>
        )}
      </div>
    </div>
  );
}

// ─── Main App ──────────────────────────────────────────────────────────────────
export default function App() {
  const [scores, setScores] = useState(() => retrieve(STORAGE_KEYS.scores, {}));
  const [journal, setJournal] = useState(() => retrieve(STORAGE_KEYS.journal, {}));
  const [goals, setGoals] = useState(() => retrieve(STORAGE_KEYS.goals, {}));
  const [answers, setAnswers] = useState(() => retrieve(STORAGE_KEYS.answers, {}));
  const [userName, setUserName] = useState(() => retrieve(STORAGE_KEYS.name, ""));
  const [active, setActive] = useState(null);
  const [mounted, setMounted] = useState(false);
  const [nameInput, setNameInput] = useState("");
  const [showNamePrompt, setShowNamePrompt] = useState(false);

  useEffect(() => {
    setTimeout(() => setMounted(true), 80);
    if (!retrieve(STORAGE_KEYS.name, "")) setShowNamePrompt(true);
  }, []);

  const handleScore = (id, s) => { const u = { ...scores, [id]: s }; setScores(u); store(STORAGE_KEYS.scores, u); };
  const handleJournal = (id, e) => { const u = { ...journal, [id]: e }; setJournal(u); store(STORAGE_KEYS.journal, u); };
  const handleGoals = (id, g) => { const u = { ...goals, [id]: g }; setGoals(u); store(STORAGE_KEYS.goals, u); };
  const handleAnswers = (id, a) => { const u = { ...answers, [id]: a }; setAnswers(u); store(STORAGE_KEYS.answers, u); };

  const handleNameSubmit = () => {
    if (!nameInput.trim()) return;
    setUserName(nameInput.trim());
    store(STORAGE_KEYS.name, nameInput.trim());
    setShowNamePrompt(false);
  };

  const scored = DOMAINS.filter(d => scores[d.id] > 0);
  const avg = scored.length > 0 ? Math.round(scored.reduce((a, d) => a + scores[d.id], 0) / scored.length * 10) / 10 : null;
  const totalGoals = DOMAINS.reduce((a, d) => a + (goals[d.id]?.length || 0), 0);
  const completedGoals = DOMAINS.reduce((a, d) => a + (goals[d.id]?.filter(g => g.done).length || 0), 0);

  return (
    <div style={{ minHeight: "100vh", background: "#0E0B08" }}>
      <div style={{ position: "fixed", inset: 0, zIndex: 0, pointerEvents: "none", background: `radial-gradient(ellipse 60% 40% at 15% 0%, rgba(196,120,42,0.08) 0%, transparent 70%), radial-gradient(ellipse 50% 40% at 85% 100%, rgba(91,143,168,0.06) 0%, transparent 70%)` }} />

      <div style={{ position: "relative", zIndex: 1, maxWidth: "960px", margin: "0 auto", padding: "48px 24px 80px" }}>

        {/* Name Prompt */}
        {showNamePrompt && (
          <div style={{
            position: "fixed", inset: 0, zIndex: 300, background: "rgba(8,6,4,0.96)",
            display: "flex", alignItems: "center", justifyContent: "center",
            padding: "24px", backdropFilter: "blur(8px)"
          }}>
            <div style={{ background: "#141008", border: "1px solid rgba(196,120,42,0.3)", borderRadius: "24px", padding: "48px 40px", maxWidth: "440px", width: "100%", textAlign: "center" }}>
              <div style={{ fontSize: "32px", marginBottom: "16px" }}>◈</div>
              <h2 style={{ fontFamily: "'Cormorant Garamond', serif", fontSize: "28px", color: "#F5ECD7", marginBottom: "10px" }}>Welcome to Origins Unity</h2>
              <p style={{ color: "rgba(245,236,215,0.5)", fontSize: "14px", lineHeight: "1.6", marginBottom: "28px" }}>
                Your personal wellness platform across 8 domains of life. Let's start with your name.
              </p>
              <input autoFocus value={nameInput} onChange={e => setNameInput(e.target.value)}
                onKeyDown={e => e.key === "Enter" && handleNameSubmit()}
                placeholder="Your first name"
                style={{
                  width: "100%", padding: "14px 18px", background: "rgba(255,255,255,0.06)",
                  border: "1px solid rgba(255,255,255,0.12)", borderRadius: "12px",
                  color: "#F5ECD7", fontSize: "16px", outline: "none", marginBottom: "14px",
                  fontFamily: "'DM Sans', sans-serif", textAlign: "center", boxSizing: "border-box"
                }}
              />
              <button onClick={handleNameSubmit} style={{
                width: "100%", padding: "14px", background: "#C4782A", border: "none",
                borderRadius: "12px", color: "#fff", fontSize: "15px", fontWeight: "600",
                cursor: "pointer", letterSpacing: "0.03em"
              }}>Begin My Wellness Journey →</button>
            </div>
          </div>
        )}

        {/* Header */}
        <div style={{ textAlign: "center", marginBottom: "52px", opacity: mounted ? 1 : 0, transform: mounted ? "none" : "translateY(24px)", transition: "all 0.9s cubic-bezier(.4,0,.2,1)" }}>
          <div style={{ fontSize: "11px", letterSpacing: "0.35em", color: "#C4782A", textTransform: "uppercase", marginBottom: "14px", fontWeight: "500" }}>Origins Unity</div>
          <h1 style={{ fontFamily: "'Cormorant Garamond', serif", fontSize: "clamp(32px, 6vw, 54px)", fontWeight: "700", color: "#F5ECD7", margin: "0 0 10px", lineHeight: "1.15" }}>
            {userName ? `${userName}'s Wellness Landscape` : "Your Wellness Landscape"}
          </h1>
          <p style={{ fontSize: "15px", color: "rgba(245,236,215,0.45)", fontStyle: "italic", margin: 0 }}>Eight domains. One life. All yours.</p>

          {(avg !== null || totalGoals > 0) && (
            <div style={{ display: "inline-flex", alignItems: "center", gap: "24px", marginTop: "24px", padding: "14px 28px", background: "rgba(196,120,42,0.08)", border: "1px solid rgba(196,120,42,0.2)", borderRadius: "100px", flexWrap: "wrap", justifyContent: "center" }}>
              {avg !== null && (<>
                <div style={{ textAlign: "center" }}>
                  <div style={{ fontSize: "22px", fontFamily: "'Cormorant Garamond', serif", fontWeight: "700", color: "#C4782A" }}>{avg}/10</div>
                  <div style={{ fontSize: "10px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.1em" }}>Avg Score</div>
                </div>
                <div style={{ width: "1px", height: "32px", background: "rgba(255,255,255,0.1)" }} />
                <div style={{ textAlign: "center" }}>
                  <div style={{ fontSize: "22px", fontFamily: "'Cormorant Garamond', serif", fontWeight: "700", color: "#C4782A" }}>{scored.length}/8</div>
                  <div style={{ fontSize: "10px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.1em" }}>Domains Rated</div>
                </div>
              </>)}
              {totalGoals > 0 && (<>
                <div style={{ width: "1px", height: "32px", background: "rgba(255,255,255,0.1)" }} />
                <div style={{ textAlign: "center" }}>
                  <div style={{ fontSize: "22px", fontFamily: "'Cormorant Garamond', serif", fontWeight: "700", color: "#C4782A" }}>{completedGoals}/{totalGoals}</div>
                  <div style={{ fontSize: "10px", color: "rgba(245,236,215,0.4)", textTransform: "uppercase", letterSpacing: "0.1em" }}>Actions Done</div>
                </div>
              </>)}
            </div>
          )}
        </div>

        {/* Domain Grid */}
        <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill, minmax(280px, 1fr))", gap: "16px" }}>
          {DOMAINS.map((domain, i) => (
            <div key={domain.id} style={{ opacity: mounted ? 1 : 0, transform: mounted ? "none" : "translateY(32px)", transition: `all 0.65s cubic-bezier(.4,0,.2,1) ${0.1 + i * 0.075}s` }}>
              <DomainCard domain={domain} score={scores[domain.id] || 0} onClick={() => setActive(domain)} index={i} />
            </div>
          ))}
        </div>

        {scored.length === 0 && mounted && (
          <div style={{ textAlign: "center", marginTop: "40px", color: "rgba(245,236,215,0.3)", fontSize: "14px", fontStyle: "italic" }}>
            Tap any domain to begin your wellness assessment →
          </div>
        )}

        <div style={{ textAlign: "center", marginTop: "72px" }}>
          <div style={{ fontSize: "20px", color: "rgba(196,120,42,0.4)", marginBottom: "8px" }}>◈</div>
          <div style={{ fontSize: "12px", color: "rgba(245,236,215,0.2)", letterSpacing: "0.08em" }}>Origins Unity · Fatigue to Fit · Built for builders</div>
        </div>
      </div>

      {active && (
        <DomainModal
          domain={active}
          score={scores[active.id] || 0}
          onScore={handleScore}
          onClose={() => setActive(null)}
          journal={journal}
          onJournal={handleJournal}
          goals={goals}
          onGoals={handleGoals}
          answers={answers}
          onAnswers={handleAnswers}
        />
      )}
    </div>
  );
}
