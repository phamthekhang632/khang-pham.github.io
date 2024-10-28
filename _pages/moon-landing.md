---
layout: default
title: "Landing Space Shuttle using Deep Q-Learning"
permalink: /moon-landing/
author_profile: true
classes: wide
---

<div style="text-align: center; margin-bottom: 30px;">
  <img src="{{ site.baseurl }}/assets/images/moon-landing_environment.png" alt="XPRIZE Rainforest" style="max-width: 100%; height: auto; border-radius: 15px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);">
</div>

# Landing Space Shuttle using Deep Q-Learning

This was my first attempt to learn reinforcement learning. The agent was trained to land a space shuttle in a randomly generated environment.

I started by learning Q-Learning through a project on solving Black Jack. However, because of the finite dimension limitation, I decided to use Deep Q-Learning, which combined the original method with a neural network. This approach showed promising results. 

<div style="display: flex; justify-content: center; gap: 20px; margin-bottom: 30px;">
  <div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/images/moon-landing_reward.png" alt="XPRIZE Rainforest 1" style="max-width: 100%; height: auto; border-radius: 15px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);">
  </div>

  <div style="text-align: center;">
    <img src="{{ site.baseurl }}/assets/images/moon-landing_duration.png" alt="XPRIZE Rainforest 2" style="max-width: 100%; height: auto; border-radius: 15px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);">
  </div>
</div>

As shown above, after about 200 episodes, the agent learned how to land the shuttle reliably. Additionally, since I added the punishment for using too much fuel, the agent also learned to land the shuttle more confidently (200 frames vs. 900 frames). 

For this project, I had to learn how to use PyTorch and implement different reinforcement learning algorithms in two weeks.

<div style="text-align: center; margin-top: 30px;">
  <a href="{{ site.baseurl }}/" class="btn btn-home">Back to Home</a>
</div>