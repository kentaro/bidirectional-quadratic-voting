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
  /* 三重引用を脚注の記号に転用 */
  /* 下記はdefaultテーマ用。他のテーマで利用するときはbottomとleftを調節してください。 */
  /* スライド全体で利用するため、無名のstyleタグを利用しています。 */
  blockquote > blockquote > blockquote {
    font-size: 40%;
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

# Potential Solution:<br>Quadratic Voting (QV)

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

# Candidate Preferences

- Candidates span political spectrum
- Candidate 2: tech expert

![Candidate Distribution](./images/candidates.png)

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 100%;
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

# Simulation Results (*1)

- Balanced results vs. normal voting
- Higher support for tech-expert candidate

![Simulation Results](./images/simulation-results.png)

>>> *1: Only results for normal distribution shown

<style scoped>
  img {
    display: block;
    margin: auto;
    width: 50%;
  }
</style>

---

# Conclusion

- QV/BQV is a promising mechanism for social implementation on Ethereum
- GMO aims to collaborate with the Ethereum community to create positive social impact
- Together, we can leverage blockchain technology to build a better world
