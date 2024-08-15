---
marp: true
theme: default
paginate: true
style: |
  section {
    font-size: 36pt;
    background-image: url('images/pepabo.png');
    background-position: top right;
    background-repeat: no-repeat;
    background-size: 15%;
  }
  h1 {
    font-size: 48pt;
    margin-bottom: 36pt;
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
  padding-bottom: 0;
}
h2 {
  margin-top: 0;
}
section {
  font-size: 24pt;
}
</style>

---


# About Me

- Kentaro Kuribayashi
- CTO at GMO Pepabo, Inc.
- [kentarokuribayashi.com](https://kentarokuribayashi.com)

![bg right:35% height:50%](https://pbs.twimg.com/profile_images/1737743542724997120/ygmW433p_400x400.jpg)

---

# Challenge: The Voting Dilemma

![background](./images/background.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 80%;
  }
</style>

---

# Potential Solution:<br>Quadratic Voting (QV)

- Express varying preference strengths
- Quadratic credit allocation
- Amplifies minority opinions

![bg right:35% height:65%](./images/qv.png)

---

# Applying QV to Elections

![Appling QV to Elections](./images/applying-qv-to-elections.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 100%;
  }
</style>
---

# Proposed Solution:<br>Bidirectional Quadratic Voting (BQV)

## Challenge
- QV alone may not achieve precise matching with candidate preferences

## New Proposal: Bidirectional Quadratic Voting
- Both voters and candidates use QV
- Achieves more accurate preference matching

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
