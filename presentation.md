---
marp: true
theme: default
paginate: true
style: |
  section {
    font-size: 36pt;
  }
  h1 {
    font-size: 48pt;
  }
  h2 {
    font-size: 42px;
  }
---

# Bidirectional Quadratic Voting
## A Proposal for Precise Candidate Matching

Kentaro Kuribayashi
GMO Pepabo, Inc.

<style scoped>
h1 {
  margin-bottom: 0;
}
h2 {
  margin-top: 0;
}
section {
  font-size: 24pt;
}
</style>

---

# Background

- Diverse candidate policy preferences
- Dilemma: Experience vs. New technology
- Limitations of conventional voting:
  - Single vote ≠ Multiple preferences
  - Minority opinions often overlooked

---

# Current Challenges

1. Can't support both established and tech-focused candidates
2. Complex voter preferences not fully expressed
3. Risk of weakening support for viable candidates

---

# Simulation Setup

- 5 candidates (-1 to 1 ideology scale)
- 7 policy issues (incl. technology & performance)
- 10,000 simulated voters
- 4 voter distributions tested

---

# Key Assumptions

1. Fixed candidate preferences
2. Voter preferences based on ideology + randomness
3. 50% prioritize political performance
4. 5% strongly prioritize technology
5. Social influence affects preferences

---

# Proposed Solution: Quadratic Voting (QV)

- Express varying preference strengths
- Quadratic credit allocation
- Amplifies minority opinions

---

# Bidirectional Quadratic Voting

## Challenge
- QV alone may not achieve precise matching with candidate preferences

## New Proposal: Bidirectional Quadratic Voting
- Both voters and candidates use QV
- Achieves more accurate preference matching

---

# Simulation Process

1. Generate preferences (candidates & voters)
2. Calculate scores for 3 voting methods
3. Compare and visualize results

---

# Simulation Results

![Simulation Results](https://example.com/simulation_results.png)

- Comparison of normal voting, QV, and bidirectional QV
- Verification across various voter distribution patterns

---

# Key Findings

1. Bidirectional QV shows more balanced results across different voter distributions
2. QV and Bidirectional QV give more weight to minority opinions compared to normal voting
3. The impact of voting method varies depending on the voter ideology distribution

---

# Conclusion

- Bidirectional QV more accurately reflects complex preferences
- Supports major candidates without compromising technology-focused opinions
- Suitable voting system for societies with diverse policy preferences

---

# Future Challenges

- Implementation and verification in actual elections
- Voter education and development of user-friendly interfaces
- Consideration of legal and ethical aspects
- Further refinement of the simulation model
