# Phishing & Pragmatics: NLP Seminar Project (AAU WS 2026/27)

Partner A: Nils;
Partner B: Pavel

**Roles:**
- **Partner A:** Linguistics & Data
- **Partner B:** LLM Input & Evaluation

## Step 1: Frame 
- [ ] **[Partner A]** Define linguistic phenomena (coercive modality, urgent deixis, disguised speech acts) and select textbook examples.
- [ ] **[Partner B]** Define NLP task family (classification + span extraction) and target metrics (Precision, Recall, F1).

## Step 2: Data 
- [ ] **[Partner A]** Collect 40–60 anonymized emails (phishing + legitimate "hard negatives" like real university deadlines).
- [ ] **[Partner A]** Write `data/annotation_guideline.md` *before* testing any LLM outputs and document 1 ambiguous case.
- [ ] **[Partner A]** Hand-annotate the gold standard labels and cue spans.
- [ ] **[Partner B]** Split corpus into `dev_set.json` and `test_set_FROZEN.json` and document split stats.

## Step 3: Baseline 
- [ ] **[Partner A]** Supply linguistic trigger word/pattern list for the transparent baseline.
- [ ] **[Partner B]** Implement `evaluation/baseline.py` and record baseline Precision, Recall, and F1.

## Step 4: LLM Input 
- [ ] **[Partner B]** Write Prompt v1, then iterate to v2 and v3 on the Dev set using Gricean maxims and structured output rules.
- [ ] **[Partner A]** Review prompt wording for linguistic clarity and unambiguous definitions.
- [ ] **[Partner B]** Log full prompt texts, model version, temperature, and token counts in `prompts/prompt_log.md`.

## Step 5: Evaluate 
- [ ] **[Partner B]** Run final evaluation on `test_set_FROZEN.json` and generate metrics table (classification + cue extraction).
- [ ] **[Partner A]** Lead qualitative error analysis in `evaluation/error_analysis.md` (missed cues, false positives on benign urgency).
- [ ] **[Both]** Review all evaluation results and verify edge cases together.

## Step 6: Document & App Concept 
- [ ] **[Partner A]** Document privacy, bias, and limitations (e.g., German vs. English phishing, text-only limits).
- [ ] **[Partner B]** Build clickable Phishing Trainer prototype in `app/` using the winning v3 agent prompt.
- [ ] **[Both]** Finalize the 15-slide report and verify every claim is backed by data.
- [ ] 
