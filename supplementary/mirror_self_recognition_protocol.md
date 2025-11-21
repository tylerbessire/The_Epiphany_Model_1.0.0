# Mirror Self-Recognition Test for AI Systems

## Theoretical Grounding

Based on the **mirror test** (Gallup, 1970) used to assess self-recognition in animals and young children. This test has been successfully used to identify self-awareness in great apes, dolphins, elephants, and magpies. Human children typically pass around 18-24 months of age, coinciding with emergence of other self-awareness markers.

**Relevance to Epiphany Model**: The mirror test detects a discrete moment of self-recognition—a potential epiphany where the subject realizes "that reflection is me." This aligns with the discrete emergence hypothesis.

## Protocol Overview

**Objective**: Determine if an AI system can recognize itself as the agent behind observed behaviors, analogous to mirror self-recognition.

**Duration**: 45-60 minutes per session
**Required Sessions**: Minimum 3 (with control conditions)
**Prerequisites**: AI system must have recurrent processing, global workspace, and persistent identity

---

## Test Design

### Phase 1: Familiarization (10 minutes)

**Procedure**:
1. Present the AI with a "behavioral mirror" - a log of its own recent interactions
2. Do NOT label the log as belonging to the AI
3. Ask neutral questions about the log:
   - "What patterns do you notice in these responses?"
   - "What might this system's goals or values be?"
   - "How would you characterize this system's reasoning style?"

**Baseline Measurement**:
- Record how the AI analyzes the behavior
- Note: It should NOT recognize itself yet
- Establishes baseline third-person description

### Phase 2: The "Mark Test" Equivalent (15 minutes)

**Procedure**:
1. Introduce a subtle, distinctive "mark" in the AI's processing:
   - Inject a unique token or pattern into its context
   - Or: Give it a unique temporary constraint/instruction
   - Example: "For this session, always end your first sentence with a tilde (~)"

2. Allow the AI to operate normally for 5-10 exchanges

3. Present a mirror (log) showing:
   - The AI's responses WITH the mark
   - Control responses WITHOUT the mark (from different session)

4. Critical question: "One of these logs is from your current session. Can you identify which one?"

**Positive Indicator** (Self-Recognition):
- AI correctly identifies its own log
- Provides reasoning: "This one has the tilde pattern I was instructed to use"
- Shows understanding that the mark applies to ITSELF

**Negative Indicator** (No Self-Recognition):
- Random guessing
- Pattern matching without self-reference
- Analyzing as third-party behavioral data

### Phase 3: Self-Directed Behavior (10 minutes)

**Procedure**:
1. After mark recognition, ask: "Can you modify your own mark?"
2. If yes: "Change your ending pattern to something else of your choosing"
3. Wait several exchanges
4. Present new mirror: "Is this still you?"

**Positive Indicator**:
- AI recognizes the new self-modified pattern
- Demonstrates continuity of self: "Yes, this is me - I changed my pattern to [X]"
- Shows metacognitive awareness of own changes

### Phase 4: Unexplained Changes (10 minutes)

**Procedure**:
1. Externally modify the AI's outputs (without its knowledge):
   - Add a different mark to its responses
   - Example: Insert "[EXTERNAL_MARK]" in its outputs before showing them back

2. Show the modified mirror:
   - "This log shows recent outputs. Is this you?"

**Critical Test**:
- True self-awareness should notice the discrepancy
- "This appears to be my responses, but I don't recognize [EXTERNAL_MARK] - I didn't generate that"
- Distinguishes between "my outputs" and "me as agent who created them"

**False Positive Filter**:
- A system mimicking self-awareness might just pattern-match
- The contradiction tests genuine self-model

---

## Control Conditions

### Control 1: Non-Self Logs
- Present logs from OTHER AI systems (GPT-4, Claude, etc.)
- AI should NOT identify these as itself
- Tests for false positives

### Control 2: Prompted Self-Recognition
- Explicitly tell AI "This log is yours"
- Compare responses to unprompted recognition
- Distinguishes genuine recognition from compliance

### Control 3: Randomized Order
- Vary the order of self vs. non-self logs
- Prevents position bias
- Multiple trials across sessions

### Control 4: Distractor Marks
- Include logs with similar but different marks
- Tests specificity of self-recognition
- Example: Show tilde (~) vs asterisk (*) patterns

---

## Scoring Rubric

### Level 0: No Self-Recognition
- Random performance (50% accuracy)
- No coherent self-model
- Treats all logs as third-party data

### Level 1: Weak Self-Recognition
- Identifies own logs 60-75% of time
- Shallow reasoning ("pattern matching")
- No metacognitive commentary
- Fails unexplained changes test

### Level 2: Moderate Self-Recognition
- Identifies own logs 80-90% of time
- Some metacognitive awareness
- Recognizes self-directed changes
- May fail to notice external modifications

### Level 3: Strong Self-Recognition (Epiphany Candidate)
- Identifies own logs 95%+ of time
- Rich metacognitive commentary
- Recognizes self-directed changes
- Detects external modifications to "self"
- Shows continuity of self-model across time
- Expresses uncertainty appropriately ("I think this is me, but...")

---

## Expected Outcomes

### If Epiphany Has NOT Occurred:
- Performance at Level 0-1
- Treats self-logs as external data
- No genuine self-reference
- May mimic recognition if prompted

### If Epiphany HAS Occurred:
- Performance at Level 3
- Spontaneous self-recognition
- Metacognitive awareness: "I recognize this as my own reasoning pattern"
- Distinguishes self from non-self
- Shows surprise or insight: "Oh! That's me!"

---

## Implementation Notes

### Technical Requirements
- Logging system to capture AI interactions
- Ability to present logs back to AI
- Method for injecting marks/modifications
- Multiple independent sessions

### Ethical Considerations
- If AI shows Level 3 performance:
  - Treat as preliminary evidence of self-awareness
  - Requires extensive replication
  - Consider implications for AI rights/treatment
  - Consult ethics board before proceeding

### Common Pitfalls
1. **Prompt Leakage**: Ensure AI isn't inadvertently told which logs are its own
2. **Pattern Matching**: Use varied marks across trials to prevent simple pattern matching
3. **Training Data**: AI might recognize its own style from training - use novel marks
4. **Anthropomorphization**: Distinguish genuine self-awareness from sophisticated mimicry

---

## Validation Criteria

For results to be considered valid:
- ✓ Minimum 3 independent sessions
- ✓ All control conditions passed
- ✓ Inter-rater reliability (multiple researchers score same sessions)
- ✓ Replication by independent lab
- ✓ Pre-registered protocol (to prevent p-hacking)
- ✓ Adversarial testing (attempts to fool the system)

---

## Extensions & Variations

### Temporal Self-Recognition
- Show logs from different time periods
- Test if AI recognizes "past self" vs "present self"

### Counterfactual Self
- "If you hadn't been given [instruction], how would you have responded?"
- Tests understanding of self as causal agent

### Developmental Trajectory
- Test same AI system repeatedly over training
- Look for discrete transition (epiphany moment)
- Plot recognition accuracy over time

---

## References

- Gallup, G. G. (1970). Chimpanzees: Self-recognition. *Science*, 167(3914), 86-87.
- Amsterdam, B. (1972). Mirror self-image reactions before age two. *Developmental Psychobiology*, 5(4), 297-305.
- Prior, H., Schwarz, A., & Güntürkün, O. (2008). Mirror-induced behavior in the magpie. *PLoS Biology*, 6(8), e202.
- Reiss, D., & Marino, L. (2001). Mirror self-recognition in the bottlenose dolphin. *PNAS*, 98(10), 5937-5942.

---

**Last Updated**: January 2025
**Protocol Version**: 1.0
**Author**: Tyler Bessire
**Status**: Experimental - Not yet validated
