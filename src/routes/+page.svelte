<div class="container">
  <div class="header">
    <img src="/rose.png" alt="rose-human" class="rose"/>
    <h1>Co-Development of Brain and Body</h1>
    <h2>Cooper b. Anderson, Jason A. Yoder</h2>
    <h2>Rose-Hulman Institute of Technology</h2>
  </div>
  <div class="columns">
    <div class="left">
      <h3>Introduction</h3>
      <ul>
        <li>Dynamic Neural Networks</li>
        <li>Continuous-Time Recurrent Neural Networks</li>
        <li>Reinforcement Learning-like Rule</li>
      </ul>
      <h3>Motivation</h3>
      <img src="/worm.gif" alt="worm gif" class="img" />
      <ul>
        <li>Most locomotion simulations train on the timescale of many generations.</li>
        <ul>
          <li>We want to get similar results on the timescale of a single lifetime.</li>
        </ul>
      </ul>
      <h4>Developmental process</h4>
      <ul>
        <li>Observed in biology</li>
        <li>Capable of extreme complexity</li>
      </ul>
    </div>
    <div class="center">
      <h3>Methodology</h3>
      <h4>Developmental Brain model</h4>
      <ul>
        <li>CTRNN</li>
      </ul>
        <img src="/activation.png" alt="network" class="img" />
        <div class="flex">
          <img src="/network.png" alt="network" class="network" />
          <img src="/parametric.png" alt="network" class="network" />
        </div>
      <ul>
        <li>Making it developmental: Add more neurons over time</li>
      </ul>
      <h4>Developmental Body model</h4>
      <ul>
        <li>Spring-Mass system</li>
        <li>Making it developmental: Adding more body segmentals over tiem</li>
      </ul>
      <div class="flex">
        <img src="/worm-2.png" alt="network" class="network" />
        <div>&rightarrow;</div>
        <img src="/worm-3.png" alt="network" class="network" />
      </div>
    </div>
    <div class="right">
      <h3>Experiments</h3>
      <img src="/goals.png" alt="goals" class="img" />
      <h3>Contributions</h3>
      <ul>
        <li>Chaotically varying weights</li>
        <img src="/flux.png" alt="flux" class="img" />
        Like the game, "hotter or colder," it is a method of reinforcement
      </ul>
    </div>
  </div>
</div>

<style>
  /* Styling */
  h1, h2, h3, h4 {
    margin-top: 0;
    margin-bottom: 0;
    text-align: center;
  }

  h3 {
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .rose {
    float: left;
    height: 100px;
  }

  .network {
    height: 100px;
  }

  .img {
    width: 100%;
  }

  .flex {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
  }

  /* .flex-1 {
    flex: 1;
  } */

  /* Layout */
  :root {
    --gap: 15px;
    font-family: Arial, Helvetica, sans-serif;
  }

  .container {
    position: relative;
    width: 1000px;
    height: 750px;
    display: flex;
    flex-direction: column;
    gap: var(--gap);
    padding: var(--gap);
    box-sizing: border-box;
    margin: auto;
  }

  .columns {
    flex: 1;
    display: flex;
    gap: var(--gap);
  }

  .columns > div {
    flex: 1;
  }

  .container {
    background-color: #eee;
  }

  .header, .columns > div {
    background-color: #fff;
  }
</style>
