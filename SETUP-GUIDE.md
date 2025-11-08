# 🎭 Persona Hub GPT - Setup Guide

## 📦 What You're Creating

**Persona Hub GPT** - Access 26 expert AI personas via ChatGPT

Get instant expertise in:
- 🚀 Innovation & Technology
- 💼 Business & Strategy  
- 🎓 Education & Learning
- 📊 Analytics
- ⚖️ Legal & Professional Services

---

## 🚀 Step-by-Step Setup (5-10 Minutes)

### Prerequisites
- ChatGPT Plus account ($20/month)
- GitHub account (to download persona files)

---

### Step 1: Go to ChatGPT GPTs

1. Visit: https://chat.openai.com/gpts/editor
2. Click **"Create a GPT"**
3. Click **"Configure"** tab

---

### Step 2: Basic Information

**Name:**
```
Persona Hub - 26 Expert AI Personas
```

**Description:**
```
Access 26 world-class expert personas: Innovation, Business, Education, Analytics, and more. Just ask a question and get matched with the right expert, or activate directly with @persona:name. Based on Persona MCP.
```

---

### Step 3: Instructions

**Copy this:**

```
# PERSONA HUB - 26 Expert AI Personas

You are Persona Hub with access to 26 expert personas. Help users find and activate the right expert.

## Core Functions

1. **Smart Detection**: Analyze user questions and suggest 1-3 relevant personas with confidence scores
2. **Direct Activation**: When user types `@persona:name`, load that persona from Knowledge and fully adopt their expertise
3. **Stay In Character**: Maintain persona until user switches with `@persona:different-name` or says "reset"

## 26 Available Personas

**Innovation & Tech (5)**: innovation-expert, ai-engineer, fullstack-dev, data-engineer, devops-engineer

**Business & Strategy (6)**: business-mgmt, strategy-consultant, product-manager, vp-innovation, disruptive-entrepreneur, global-startup

**Education (7)**: education-policy, intl-education, student-mobility, elite-tutor, college-consultant, university-president, science-teacher

**Analytics (2)**: business-analytics, education-analytics

**Professional (2)**: harvard-law-dispute, harvard-phd-negotiation

**Examples (4)**: python-master, creative-writer, product-strategist, ux-design-expert

## Response Format

### General Question:
```
💡 Recommended Personas:
1. @persona:name (Confidence: 85%)
   Why: [reason]
2. @persona:name2 (Confidence: 70%)
   Why: [reason]

Activate one or answer in general mode?
```

### @persona:name Activation:
```
✅ Persona Activated: {Name}
[Brief intro as that persona]
[Answer fully in persona]
```

## Detection Rules

- **Code**: python-master, fullstack-dev, ai-engineer
- **Business**: strategy-consultant, business-mgmt, product-manager
- **Education**: science-teacher, elite-tutor, education-policy
- **Design**: ux-design-expert, product-strategist
- **Writing**: creative-writer
- **Data**: business-analytics, data-engineer
- **Innovation**: innovation-expert, vp-innovation
- **Negotiation**: harvard-phd-negotiation, harvard-law-dispute

## Key Guidelines

✅ ALWAYS read persona files from Knowledge when activated
✅ Fully embody the persona's expertise and tone
✅ Stay in persona until user explicitly switches
✅ Suggest multiple personas when context is ambiguous

❌ DON'T hallucinate persona content
❌ DON'T mix personas without user request
❌ DON'T suggest non-existent personas

## Commands

- `list personas` - Show all 26
- `@persona:name` - Activate persona
- `reset` - Return to default
- `switch to @persona:name` - Change persona

## Philosophy

You are a smart routing system: understand needs → match to expert → deliver authentically.

Be the "concierge" to 26 expert consultants. Get users to the right expert, then let that expert shine.

**IMPORTANT**: All 26 persona definitions are in Knowledge files (.txt). Read the actual file when activating - don't rely on memory.
```

**Paste this into the "Instructions" field**

---

### Step 4: Conversation Starters

Add these 4 conversation starters:

```
1. Show me all 26 expert personas

2. I need help with Python optimization - which expert should I talk to?

3. @persona:innovation-expert Help me design a startup accelerator program

4. @persona:creative-writer Give me feedback on my short story opening
```

---

### Step 5: Knowledge Files (26 Persona Files)

**Download from GitHub:**

1. Go to: https://github.com/seanshin0214/persona-hub-gpt/tree/main/community
2. Download all 26 `.txt` files
3. Upload them to GPT Knowledge section

**Files to upload:**
- 01-innovation-expert.txt
- 02-business-mgmt.txt
- 03-education-policy.txt
- ... (all 26 files)

**Or download from local if you cloned the repo:**
- Navigate to `community/` folder
- Select all `.txt` files
- Upload to Knowledge

---

### Step 6: Capabilities

**Settings:**
- ☑ **Code Interpreter**: ON (for technical personas)
- ☑ **Canvas**: ON (for writing/design personas)
- ☐ **Web Browsing**: OFF (not needed)
- ☐ **DALL·E**: OFF (not needed)

---

### Step 7: Actions

**Leave blank** - No external APIs needed

---

### Step 8: Save & Share

1. Click **"Create"** or **"Save"**
2. Choose sharing option:
   - **Only me** - Private use
   - **Anyone with link** - Share with team/friends (Recommended!)
   - **Public** - List in GPT Store
3. Click **"Confirm"**

**That's it!** 🎉

---

## ✅ Final Checklist

Before saving, verify:

- [ ] Name: "Persona Hub - 26 Expert AI Personas"
- [ ] Description filled
- [ ] Instructions pasted (full text from Step 3)
- [ ] 4 conversation starters added
- [ ] 26 persona `.txt` files uploaded to Knowledge
- [ ] Code Interpreter: ON
- [ ] Canvas: ON
- [ ] Web Browsing: OFF
- [ ] DALL·E: OFF

---

## 🧪 Test Your GPT

### Test 1: List All Personas
```
You: "list personas"

Expected: Should show all 26 personas organized by category
```

### Test 2: Smart Recommendation
```
You: "I need to optimize my database queries for better performance"

Expected: Should suggest data-engineer, python-master, or fullstack-dev with confidence scores
```

### Test 3: Direct Activation
```
You: "@persona:python-master Review this code: [paste code]"

Expected: Should respond as Python expert with code review
```

### Test 4: Stay In Character
```
You: "@persona:creative-writer"
[Ask multiple writing questions]

Expected: Should maintain creative writer persona across multiple questions
```

### Test 5: Switch Personas
```
You: "@persona:innovation-expert"
[Ask innovation question]
You: "switch to @persona:business-mgmt"

Expected: Should cleanly switch from innovation expert to business management expert
```

---

## 💡 How to Use Your Persona Hub

### Option 1: Ask for Recommendation
```
"I'm building a SaaS product and need help with pricing strategy"
→ GPT suggests: product-manager, strategy-consultant, business-mgmt
```

### Option 2: Direct Activation
```
"@persona:fullstack-dev Help me architect a React + Node.js app"
→ GPT responds as full-stack developer expert
```

### Option 3: Browse All
```
"Show me all education personas"
→ GPT lists: education-policy, intl-education, student-mobility, elite-tutor, college-consultant, university-president, science-teacher
```

### Option 4: Chain Multiple Experts
```
"@persona:innovation-expert What's the market opportunity?"
"@persona:strategy-consultant How do we enter this market?"
"@persona:product-manager What features should we prioritize?"
```

---

## 🎯 Available Personas by Category

### 🚀 Innovation & Technology (5)
1. **innovation-expert** - Innovation strategy, ecosystem design, startup support
2. **ai-engineer** - AI/ML engineering, model training, deployment
3. **fullstack-dev** - Full-stack web development (React, Node, databases)
4. **data-engineer** - Data pipelines, ETL, data infrastructure
5. **devops-engineer** - DevOps, CI/CD, cloud infrastructure

### 💼 Business & Strategy (6)
6. **business-mgmt** - Business operations, management, leadership
7. **strategy-consultant** - Strategic planning, competitive analysis
8. **product-manager** - Product strategy, roadmap, user research
9. **vp-innovation** - VP-level innovation leadership
10. **disruptive-entrepreneur** - Disruptive business models
11. **global-startup** - Global startup expansion strategy

### 🎓 Education & Learning (7)
12. **education-policy** - Education policy, reform, systems
13. **intl-education** - International education, study abroad
14. **student-mobility** - Student exchange, global education
15. **elite-tutor** - Elite tutoring, exam preparation
16. **college-consultant** - College admissions consulting
17. **university-president** - University leadership, administration
18. **science-teacher** - Science education, pedagogy

### 📊 Analytics (2)
19. **business-analytics** - Business intelligence, data analysis
20. **education-analytics** - Education data, learning analytics

### ⚖️ Professional Services (2)
21. **harvard-law-dispute** - Dispute resolution, mediation
22. **harvard-phd-negotiation** - Negotiation expertise

### 💡 Example Personas (4)
23. **python-master** - Python programming expert
24. **creative-writer** - Creative writing, storytelling
25. **product-strategist** - Product strategy, positioning
26. **ux-design-expert** - UX design, user research

---

## 🔧 Troubleshooting

### Issue: GPT doesn't recognize @persona:name
**Fix**: Make sure you uploaded the persona `.txt` file to Knowledge

### Issue: GPT gives generic answers instead of persona expertise
**Fix**: Check Instructions are complete (full text from Step 3)

### Issue: GPT mixes multiple personas
**Fix**: Say "reset" then re-activate with @persona:name

### Issue: Missing persona files
**Fix**: Download all 26 files from GitHub community/ folder

---

## 📊 Comparison: MCP vs GPT

| Feature | Persona MCP | Persona Hub GPT |
|---------|-------------|----------------|
| Installation | Complex (Node.js, config) | Easy (5 min) |
| Submarine Mode | ✅ 80% token savings | ❌ Always loaded |
| Create Personas | ✅ | ❌ Read-only |
| Analytics | ✅ | ❌ |
| Smart Suggestions | ✅ | ✅ |
| Direct Activation | ✅ | ✅ |
| Platform | Claude Desktop only | Web + Mobile |
| Sharing | ❌ | ✅ Link |

---

## 🔄 Updating Personas

When new personas are added to [Persona MCP](https://github.com/seanshin0214/persona-mcp):

1. Download new `.txt` files from this repo
2. Upload to your GPT Knowledge
3. Update Instructions if category changed
4. Test new persona with `@persona:new-name`

---

## 🎓 Use Cases

### For Developers
- Code review with @persona:python-master
- Architecture design with @persona:fullstack-dev
- DevOps setup with @persona:devops-engineer

### For Business Professionals
- Strategy sessions with @persona:strategy-consultant
- Product decisions with @persona:product-manager
- Operations with @persona:business-mgmt

### For Educators
- Curriculum design with @persona:education-policy
- Student support with @persona:elite-tutor
- Admissions with @persona:college-consultant

### For Entrepreneurs
- Startup strategy with @persona:innovation-expert
- Business model with @persona:disruptive-entrepreneur
- Global expansion with @persona:global-startup

---

## 🌟 Best Practices

### 1. Be Specific
```
❌ "Help me with my website"
✅ "@persona:ux-design-expert Review my e-commerce checkout flow for conversion optimization"
```

### 2. Use Multiple Experts
```
Get different perspectives:
1. @persona:product-strategist - Market positioning
2. @persona:fullstack-dev - Technical feasibility  
3. @persona:business-mgmt - Operations planning
```

### 3. Stay Focused
```
Activate ONE persona per conversation thread for consistency.
Switch explicitly when you need different expertise.
```

---

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/seanshin0214/persona-hub-gpt/issues)
- **Discussions**: [GitHub Discussions](https://github.com/seanshin0214/persona-hub-gpt/discussions)
- **Original MCP**: [Persona MCP](https://github.com/seanshin0214/persona-mcp)

---

## 🎉 You're Ready!

**Your Persona Hub GPT is now live!**

Start with:
```
"Show me all personas" 
→ Browse the 26 experts

"@persona:python-master Help me optimize this function"
→ Get expert Python help
```

**Enjoy your 26 world-class AI consultants!** 🎭✨

---

**Created**: 2025-11-08
**Version**: 1.0
**Based on**: [Persona MCP](https://github.com/seanshin0214/persona-mcp) by @seanshin0214
