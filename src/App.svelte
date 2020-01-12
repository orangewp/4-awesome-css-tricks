<style>
  .main {
    padding: 20px;
  }
  @keyframes radial-pulse {
    0% {
      box-shadow: 0 0 0 0px rgba(0, 0, 0, 0.5);
    }

    100% {
      box-shadow: 0 0 0 30px rgba(0, 0, 0, 0);
    }
  }
  .box1,
  .box2 {
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    width: 200px;
    height: 200px;
    margin: 10px;
    color: white;
  }
  .box1 {
    background: red;
    animation: radial-pulse 1s infinite;
  }
  .box2 {
    position: relative;
    background: blue;
    box-sizing: border-box;
  }
  .box2 div {
    width: 90px;
    height: 120px;
    background: white;
    color: black;
    position: absolute;
    left: 0;
    top: 0;
    padding: 5px;
    box-shadow: 1px 1px 10px white;
  }
  .box1:hover,
  .box2:hover {
    border: 5px solid black;
  }
</style>

<div class="main">
  <div class="box1">Content</div>
  <div class="box2">
    <div>Content</div>
  </div>
</div>
