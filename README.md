# Gambling-with-RL--WiDS
The main repo for the WiDS 2024 project - Gambling with RL

Here is the tentative timeline for the project-
### Week 1
We'll be focusing on the basics of RL and essential Python programming skills, laying the groundwork for further exploration.  <br/>
Our main aim would be to get a general intro to RL and explore the fundamentals of Markov Decision Processes (MDPs), focusing on their structure, components, and role in modeling decision-making in reinforcement learning.

### Week 2 

This week, we'll dive into basic RL algorithms, specifically Policy and Value Iteration. Our goal is to understand how these fundamental techniques help solve MDPs by iteratively improving policies and estimating value functions.
Tasks:

-Carefully read Chapter 3 of Grokking Deep Reinforcement Learning to grasp the concepts of Policy and Value Iteration.
-Solve the upcoming assignment to reinforce your understanding.

## Extra Resources:
Watch the provided video resources for a deeper understanding of [expected returns](https://www.youtube.com/watch?v=a-SnJtmBtyA&t=47s), [policies, value functions](https://www.youtube.com/watch?v=eMxOGwbdqKY), and [optimal policies](https://www.youtube.com/watch?v=rP4oEpQbDm4&t=309s). These will complement the reading and help clarify key concepts.

### Week 3  
This week, we'll explore **Model-Free Prediction** techniques in Reinforcement Learning, specifically focusing on **Monte Carlo (MC) methods**. These methods estimate value functions using sampled experiences instead of relying on a complete model of the environment.  

**Theory:**  
- Before starting the chapter, read **Section 2.1 and the beginning of 2.2 (Page 9,10)** from the provided [resource](https://www.google.com/url?q=https://iitbacin-my.sharepoint.com/:b:/g/personal/22b0958_iitb_ac_in/EVlWfRNoMqROrnXfGyRIi-EB-HvVnbCaUIVFyU370Ui33Q?e%3DXS5RsU&sa=D&source=docs&ust=1738277581603118&usg=AOvVaw0-BX6zFluztLP89M9SKL7m).  
- Then, carefully read **Chapter 4 of *Grokking Deep Reinforcement Learning*** and solve the upcoming assignment. This chapter covers Monte Carlo methods, including first-visit and every-visit MC, and how they help estimate value functions.  

**Extra Resources:**  
- Read the provided [page](https://ai.stackexchange.com/questions/23773/why-is-regret-so-defined-in-mabs) to learn more about the **regret function**, a key concept in RL.  
- After completing *Grokking*, further strengthen your understanding by reading **Chapter 2 from *Sutton and Barto***, which provides additional insights into Monte Carlo methods and their applications.  

### Week 4  
This week, we officially start **gambling in RL** with **Blackjack**! We’ll explore **Temporal Difference (TD) learning**, a powerful method that generalizes Monte Carlo learning and allows for more flexible policy evaluation.  

**Theory:**  
- Carefully read **Chapter 5 of *Grokking Deep Reinforcement Learning*** and solve the upcoming assignment.  

**Assignment:**  
- Before training your RL agent to play **Blackjack**, play the game yourself to get familiar with its rules. Read the official documentation to understand the gameplay.  
- We’ll use the **Gym library’s “Blackjack-v1” environment** to implement **TD-learning**.  
- While **Monte Carlo methods** require complete episode rollouts, TD-learning updates value estimates **in an online fashion**, making it more efficient.  
- The **λ parameter** in TD-learning allows for flexibility:  
  - Setting **λ = 1** recovers **Monte Carlo learning**.  
  - Experiment with different **λ** values to understand their impact on policy learning.  

**Implementation:**  
- The **helper code** is already provided in the notebook—just run the initial cells.  
- Implement the **BlackjackTDAgent** class to train your RL agent.  
- Finally, **watch your agent play Blackjack** and (hopefully) win loads of money—if only it were real! 💰😆  


### Week 5 (Optional)  
This week marks our transition into **real-world-like RL problems**. Unlike the earlier phases, which had small and well-defined action and state spaces, we now delve into **complex environments** where Deep Learning enables us to train **Deep Reinforcement Learning (DRL) networks** to handle **high-dimensional state spaces and continuous action spaces**.  

---

### **So What’s Ahead?**  
Previously, we explored **Value Iteration (VI), Policy Iteration (PI), and basic Q-Learning**—fundamental concepts in RL. However, these methods **struggle to scale** to large or infinite state spaces. To tackle this, we introduce **function approximation** techniques using **Neural Networks**, which form the backbone of **Deep RL**.  

#### **Q-Networks (DQN)**  
A neural network is used to **approximate the Q-value function**, enabling us to handle large state spaces, such as **raw pixels from Atari games**.  

While other techniques like **Policy Gradient & Actor-Critic** exist, we will **focus on DQN and similar methods for now**.  

---

### **For Those New to ML & Neural Networks**  
- Start by watching this [**introductory video**]() to understand **Neural Networks** (NNs).  
- You can initially treat **Neural Nets as Black Box Function Approximators** and dive deeper later.  

---

### **Resources to Watch & Read**  
1. **Q-Learning vs Deep Q-Learning** + **Slippery Frozen Lake using DQN** [video](https://www.youtube.com/watch?v=SgC6AZss478)
2. **OG DRL Paper Explanation** - [paper](https://www.youtube.com/watch?v=nOBm4aYEYR4)  
3. **Dueling DQN - Full Implementation Playlist** - [Playlist](https://www.youtube.com/watch?v=EUrWGTCGzlA)  

---

### **What to Implement?**  
By now, you should be comfortable working with **DQN**. Using the **Frozen Lake DQN template**, your tasks are:  
- **Implement the Gymnasium Lunar-Lander environment using DQN**  
- **Solve Atari Breakout**  

**For Reference:**  
- A **Cart Pole** environment with a **solved implementation** is available in the repo. Use it as a guide.  

