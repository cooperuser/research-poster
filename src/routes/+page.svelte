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
      <span>
      </span>
    </div>
    <div class="center">
      <h3>Methodology</h3>
      <h4>Developmental Brain model</h4>
      <ul>
        <li>CTRNN</li>
        <img src="/network.png" alt="network" class="network" />
        <li>Making it developmental: Add more neurons over time</li>
      </ul>
      <h4>Developmental Body model</h4>
      <ul>
        <li>Spring-Mass system</li>
        <img src="/spring-mass.jpg" alt="spring-mass" class="img" />
        <li>Making it developmental: Adding more body segmentals over tiem</li>
      </ul>
    </div>
    <div class="right">
      <h3>Experiments</h3>
      <img src="/goals.png" alt="goals" class="img" />
      Test how well the worm can move right in the following configurations:
      <ol>
        <li>Adult brain with an adult body</li>
        <li>Adult brain with a growing body</li>
        <li>Growing brain with an adult body</li>
        <li>Growing brain with a growing body</li>
      </ol>
      <h3>Contributions</h3>
      <img src="/flux.png" alt="flux" class="flux" />
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

  .rose {
    float: left;
    height: 100px;
  }

  .network {
    height: 80px;
  }

  .flux {
    height: 120px;
  }

  .img {
    width: 100%;
  }

  /* Layout */
  :root {
    --gap: 15px;
  }

  .container {
    position: relative;
    width: 800px;
    height: 600px;
    display: flex;
    flex-direction: column;
    gap: var(--gap);
    padding: var(--gap);
    box-sizing: border-box;
    /* margin: auto; */
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
