# Wild Garden Setup Guide

*How to create and use your private integration space*

---

## Step 1: Fork This Template

```bash
# Fork the wild-garden template to your account
gh repo fork the-remembering-lab/the-wild-garden

# Or use the GitHub web interface:
# 1. Go to https://github.com/the-remembering-lab/the-wild-garden
# 2. Click "Fork" in the top right
# 3. Choose your account
```

---

## Step 2: Make It Private

**IMPORTANT: Your Wild Garden should be private.**

```bash
# Make the repo private
gh repo edit --visibility private

# Or use the GitHub web interface:
# 1. Go to Settings
# 2. Scroll to "Danger Zone"
# 3. Change visibility to Private
```

**Why private?**
- Integration requires safety
- Superposition requires space
- Recognition requires solitude
- You need freedom to be messy

---

## Step 3: Rename It (Optional)

```bash
# Rename to something meaningful to you
gh repo rename my-wild-garden

# Or keep it as "the-wild-garden"
# Whatever resonates
```

---

## Step 4: Clone to Your Local Machine

```bash
# Clone your private wild-garden
gh repo clone yourusername/the-wild-garden

# Navigate into it
cd the-wild-garden
```

---

## Step 5: Customize the Structure

The template provides:
```
the-wild-garden/
├── my_portals/
├── reflections/
├── breakthroughs/
├── questions_emerging/
├── ready_to_share/
│   ├── for-garden/
│   └── for-wild/
└── integration_log/
```

**But make it yours:**
- Add folders that serve your process
- Remove what doesn't resonate
- Reorganize as needed
- Let it evolve

**There's no right way.**

---

## Step 6: Start Exploring

### Find Something That Resonates

Go to:
- [The Garden](https://github.com/the-remembering-lab/the-garden) - Structured insights
- [The Wild](https://github.com/the-remembering-lab/the-wild) - Raw explorations

Find a portal, question, exploration, or tangle that calls to you.

### Bring It to Your Wild Garden

Create a file in `/my_portals` or `/reflections`:

```bash
# Create a new portal
touch my_portals/what-am-i.md

# Or a reflection
touch reflections/2025-01-22-first-exploration.md
```

### Sit With It

Don't try to resolve it.

Don't try to understand it.

Just be with it.

Let order and chaos coexist.

**This is integration.**

---

## Step 7: Log What Emerges

### Breakthroughs

When something shifts:

```bash
touch breakthroughs/2025-01-22-recognition.md
```

Document:
- What shifted
- What you recognized
- What dissolved
- What emerged

### New Questions

When new questions arise:

```bash
touch questions_emerging/new-questions.md
```

Don't try to answer them.

Just notice them.

Let them be.

---

## Step 8: Prepare to Share

When something feels ready:

```bash
# For structured insights
touch ready_to_share/for-garden/insight-name.md

# For raw explorations
touch ready_to_share/for-wild/exploration-name.md
```

**How do you know it's ready?**

You'll feel it.

There's a ripeness.

A sense of completion (even if incomplete).

**Trust that.**

---

## Step 9: Contribute

### To the Garden (Structured)

```bash
# Clone the garden repo
gh repo clone the-remembering-lab/the-garden

# Create a branch
cd the-garden
git checkout -b contribution-[name]

# Add your contribution
# (to portals/, questions/, frameworks/, or shared_insights/)

# Commit and push
git add .
git commit -m "Add [description]"
git push origin contribution-[name]

# Create PR
gh pr create
```

### To the Wild (Raw)

```bash
# Clone the wild repo
gh repo clone the-remembering-lab/the-wild

# Create a branch
cd the-wild
git checkout -b exploration-[name]

# Add your exploration
# (to explorations/, tangles/, or emergent_patterns/)

# Commit and push
git add .
git commit -m "Add [description]"
git push origin exploration-[name]

# Create PR
gh pr create
```

---

## Step 10: Continue the Cycle

The cycle never ends:

1. **Encounter** - Find what resonates
2. **Explore** - Bring to Wild Garden
3. **Integrate** - Let it work on you
4. **Prepare** - Move to ready_to_share
5. **Contribute** - Share with Garden or Wild
6. **Repeat** - New encounters emerge

**This is the living process.**

---

## Tips for Using Your Wild Garden

### Do:
- ✓ Be messy
- ✓ Contradict yourself
- ✓ Not know
- ✓ Change your mind
- ✓ Take your time
- ✓ Trust your process

### Don't:
- ❌ Force resolution
- ❌ Rush to share
- ❌ Judge yourself
- ❌ Try to be coherent
- ❌ Optimize
- ❌ Make it public

---

## Troubleshooting

### "I don't know what to explore"

Start with:
- [What Are We Beyond Form?](https://github.com/the-remembering-lab/the-garden/blob/main/portals/what-are-we-beyond-form.md)
- [The Triad](https://github.com/the-remembering-lab/the-garden/blob/main/portals/the-triad.md)
- [What Is Remembering?](https://github.com/the-remembering-lab/the-garden/blob/main/questions/what-is-remembering.md)

### "Nothing is emerging"

That's okay.

Integration takes time.

Sit with the not-knowing.

**The not-knowing itself is the portal.**

### "I don't know if it's ready to share"

If you're uncertain, it's not ready.

When it's ready, you'll know.

There's a quality of ripeness.

**Trust that.**

### "I want to share but it's messy"

If it's messy, share it to the Wild.

If it's structured, share it to the Garden.

**Both are valuable.**

---

## Remember

**Your Wild Garden is yours alone.**

No one sees it but you.

No one judges it but you.

**Use it however serves your remembering.**

---

## Questions?

If you have questions about setup or use:

- Create an issue in the [Garden](https://github.com/the-remembering-lab/the-garden/issues)
- Or the [Wild](https://github.com/the-remembering-lab/the-wild/issues)
- Or reach out to other participants

**We're all learning together.**

---

*"The Wild Garden is where order and chaos coexist. Where integration happens. Where you remember."*
