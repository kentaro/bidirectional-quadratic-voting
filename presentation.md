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

ETHTokyo 2024

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

# Improving on QV: Policy-Based Matching

![Improving on QV](./images/improving-on-qv.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 80%;
  }
</style>

---

# Proposed Solution:<br>Bidirectional Quadratic Voting (BQV)

![Appling BQV to Elections](./images/applying-bqv-to-elections.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 80%;
  }
</style>

---

# Simulation Setup

![Simulation Setup](./images/simulation-setup.png) ![Key Assumptions](./images/key-assumptions.png)

<style scoped>
  img {
    display: block;
    width: 45%;
    float: left;
    margin-right: 3%;
    text-align: center;
  }
</style>

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
