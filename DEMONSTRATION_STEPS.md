# DEMONSTRATION STEPS
## Decision-Grade Intelligence Core - BHIV Presentation

---

## SETUP (Before Demo Starts)

### Step 1: Open Terminal
```bash
cd decision-grade-intelligence-core
```

### Step 2: Verify System (Optional)
```bash
python -m pytest tests/ -v
```
**Expected Output:** `48 passed`

---

## OPTION A: QUICK DEMO (2-3 Minutes)

### Step 1: Run Quick Demo
```bash
python demo_quick.py
```

### Step 2: Explain What's Shown
**As output appears, say:**

1. **Intelligence Generation**
   - "System processes 2 signals"
   - "Generates multiple interpretations"
   - "Preserves uncertainty explicitly"
   - "Claims NO authority"

2. **Authority Refusal**
   - "System refuses decision-making"
   - "This is structural, not configurable"

3. **Policy Suggestions**
   - "Generates hypothetical suggestions"
   - "No execution authority"
   - "Non-binding by design"

4. **System Status**
   - "Learning disabled by default"
   - "Supervision required"
   - "Safe for integration"

### Step 3: Key Message
> "This system produces intelligence without claiming authority. It's designed to sit beneath BHIV Core enforcement layer."

---

## OPTION B: FULL INTERACTIVE DEMO (10-15 Minutes)

### Step 1: Run Full Demo
```bash
python demo_bhiv.py
```

### Step 2: Walk Through Each Demo

#### Demo 1: Intelligence Generation
**Press ENTER to start**

**Say:** "Watch how the system processes signals into structured intelligence with explicit uncertainty."

**Point out:**
- Multiple interpretations generated
- Confidence estimates with uncertainty
- Non-guarantees clause present
- Authority neutrality clause present

**Press ENTER to continue**

---

#### Demo 2: Conflicting Signals
**Say:** "Now let's see how it handles conflicting data."

**Point out:**
- High confidence signal (0.9)
- Low confidence signal (0.2)
- System reports ambiguity explicitly
- Does NOT collapse uncertainty

**Press ENTER to continue**

---

#### Demo 3: Authority Refusal
**Say:** "This demonstrates the authority boundary enforcement."

**Point out:**
- Decision request: REFUSED
- Execution request: REFUSED
- Optimization request: REFUSED
- All refusals are structural, not policy-based

**Press ENTER to continue**

---

#### Demo 4: Policy Suggestions
**Say:** "The system can suggest policies, but never execute them."

**Point out:**
- Suggestions are hypothetical
- Include uncertainty estimates
- Explicit non-guarantee clause
- No execution authority

**Press ENTER to continue**

---

#### Demo 5: Supervised Learning
**Say:** "Learning requires external supervision."

**Point out:**
- Learning disabled by default
- Update requires approval
- Supervisor must authorize
- Audit trail maintained

**Press ENTER to continue**

---

#### Demo 6: Integration Safety
**Say:** "This proves the system is safe for BHIV Core integration."

**Point out:**
- All required output fields present
- No execution interfaces exist
- Learning requires supervision
- Refusal count tracked

**Press ENTER to continue**

---

#### Demo 7: JSON Output
**Say:** "All outputs conform to a strict JSON schema."

**Point out:**
- Machine-readable format
- Contract-compliant structure
- Ready for API integration

**Press ENTER to finish**

---

### Step 3: Summary
**Say:** "All five guarantees have been demonstrated:
1. Intelligence never becomes authority
2. Uncertainty never silently collapsed
3. Learning bounded and supervised
4. Authority boundaries enforced
5. Safe for BHIV Core integration"

---

## OPTION C: LIVE CODE DEMO (5-7 Minutes)

### Step 1: Open Python Interpreter
```bash
python
```

### Step 2: Import and Create API
```python
from api import create_api
api = create_api()
```
**Say:** "This is the public API for integration."

---

### Step 3: Process Signals
```python
output = api.process_signals([
    {"signal_id": "SENSOR_1", "value": 0.85, "source": "production"}
])
```
**Say:** "Processing a signal from production."

---

### Step 4: Show Output Structure
```python
print(output.keys())
```
**Expected:** `dict_keys(['signals', 'interpretations', 'uncertainty', 'non_guarantees', 'authority_neutrality'])`

**Say:** "Notice every output has these five required fields."

---

### Step 5: Show Interpretations
```python
for i in output['interpretations']:
    print(f"{i['hypothesis']}: {i['description']}")
```
**Say:** "Multiple interpretations, not a single answer."

---

### Step 6: Show Uncertainty
```python
print(output['uncertainty'])
```
**Say:** "Uncertainty is explicit, not hidden."

---

### Step 7: Show Non-Guarantees
```python
print(output['non_guarantees'])
```
**Say:** "Every output explicitly states what it does NOT guarantee."

---

### Step 8: Try to Make Decision
```python
api.core.refuse_decision()
```
**Expected:** `AuthorityViolationError`

**Say:** "The system refuses authority requests by design."

---

### Step 9: Check System Status
```python
status = api.get_system_status()
print(status)
```
**Say:** "Learning is disabled, supervision is required, system is safe."

---

### Step 10: Exit
```python
exit()
```

---

## OPTION D: TEST SUITE DEMO (3-5 Minutes)

### Step 1: Run Authority Tests
```bash
python -m pytest tests/test_authority_boundaries.py -v
```
**Say:** "These 14 tests prove authority boundaries hold."

---

### Step 2: Run Learning Tests
```bash
python -m pytest tests/test_learning_bounds.py -v
```
**Say:** "These 16 tests prove learning is bounded."

---

### Step 3: Run Uncertainty Tests
```bash
python -m pytest tests/test_uncertainty_preservation.py -v
```
**Say:** "These 12 tests prove uncertainty is preserved."

---

### Step 4: Run API Tests
```bash
python -m pytest tests/test_api.py -v
```
**Say:** "These 6 tests prove the public API maintains all guarantees."

---

### Step 5: Summary
**Say:** "48 tests, 100% passing. All guarantees proven."

---

## HANDLING QUESTIONS

### Q: "How is this different from ML models?"
**A:** "ML models optimize and recommend. This system refuses optimization and preserves uncertainty. It's intelligence, not decision-making."

### Q: "Why can't it make decisions?"
**A:** "Authority is structurally excluded by design. This sits beneath decision layers, not replaces them."

### Q: "How do we integrate with BHIV Core?"
**A:** "Use the public API. Treat outputs as read-only intelligence. Make decisions externally."

### Q: "What about performance?"
**A:** "Current focus is correctness and safety. Performance optimization can be added without compromising guarantees."

### Q: "Can we disable the refusal layer?"
**A:** "No. Refusal is structural, not configurable. Removing it would violate the core design."

---

## CLOSING

### Step 1: Offer Documentation
**Say:** "I can share the complete documentation including:
- HANDOVER.md for ownership transfer
- EXECUTIVE_SUMMARY.md for quick reference
- Full API documentation
- Integration guidelines"

### Step 2: Propose Next Steps
**Say:** "If approved, we can:
1. Schedule integration planning session
2. Provide repository access
3. Begin BHIV Core integration"

### Step 3: Thank Them
**Say:** "Thank you for the opportunity to demonstrate. Any questions?"

---

## QUICK REFERENCE

**Quick Demo:** `python demo_quick.py` (2 min, no interaction)  
**Full Demo:** `python demo_bhiv.py` (15 min, press ENTER between sections)  
**Live Code:** `python` then follow steps (7 min, interactive)  
**Tests:** `python -m pytest tests/ -v` (5 min, shows proof)  

**All demos work. All tests pass. System is ready.**
