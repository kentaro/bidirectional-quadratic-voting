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
  blockquote > blockquote > blockquote {
    font-size: 50%;
    font-weight: 400;
    padding: 0;
    margin: 0;
    border: 0;
    border-top: 0.1em solid #555;
    position: absolute;
    bottom: 10px;
    left: 10px;
  }
  
---

# Bidirectional Quadratic Voting
## Leveraging Issue-Based Matching

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

# Disclaimer

This presentation does not represent the views of my affiliated organization, nor does it reflect my personal political opinions.

---

# Challenge: The Voting Dilemma (1/2)

Balancing experience with innovation in candidate selection. 

![background](./images/challenge.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 80%;
  }
</style>

---

# Challenge: The Voting Dilemma (2/2)

- Focusing on past achievements might hinder recognition of new ideas
- Prioritizing the latter may inadvertently favor opposing candidates in reality

---

# Quadratic Voting (QV)

- QV as a potential solution
- Allows voters to express distributed preferences
- Not limited to choosing a single candidate

![bg right:35% height:65%](./images/qv.png)

---

# Applying QV to Elections

![Appling QV to Elections](./images/applying-qv-to-elections.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 95%;
  }
</style>

---

# Taking It a Step Further

- QV in elections still leaves voters uncertain about candidates' true preferences
- Need for a voting method aligning voters and candidates on specific issues

---

# Bidirectional Quadratic Voting (BQV)

![Appling BQV to Elections](./images/applying-bqv-to-elections.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 100%;
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

# Candidate Preferences

- Candidates span political spectrum
- Candidates 1 and 4: relatively high political experience
- Candidate 2: tech expert

![bg right:50% height:80%](./images/candidates.png)

<style scoped>
  section {
    font-size: 32pt;
  }
</style>

---

# Voter Distribution

- Four voter distributions assumed: normal, bimodal, left-skewed, and right-skewed
- Simulations conducted for each distribution

![Voter Distribution](./images/voter-distribution.png)

<style scoped>
  img {
    width: 100%;
  }
</style>

---

# Simulation Results (1/2)

![Simulation Results](./images/simulation-results.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 78%;
  }
</style>

---

# Simulation Results (2/2)

- QV/BQV reflects more balanced preferences compared to regular voting (*1)
- More precise modeling is needed for more accurate simulations
- For complete simulation details, please refer to my GitHub repository (*2)

>>> *1: Only results for normal distribution shown <br> *2: https://github.com/kentaro/bidirectional-quadratic-voting

<style scoped>
  section {
    font-size: 32pt;
  }
</style>

---

# Conclusion

- QV/BQV is a promising mechanism for social implementation on Ethereum
- GMO aims to collaborate with the Ethereum community to create positive social impact
- Together, we can leverage blockchain technology to build a better world!
