<template>
  <div>
    <div class="main">
      <div class="elevatorColumn"></div>
      <div class="floorsColumn">
        <div class="floor">
          <span>5</span>
          <button class="callElevator">◉</button>
        </div>
        <div class="floor">
          <span>5</span>
          <button class="callElevator">◉</button>
        </div>
        <div class="floor">
          <span>5</span>
          <button class="callElevator">◉</button>
        </div>
        <div class="floor">
          <span>5</span>
          <button class="callElevator">◉</button>
        </div>
        <div class="floor">
          <span>5</span>
          <button class="callElevator">◉</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.main {
  display: grid;
  grid-template-columns: 80px 1fr;
  grid-template-rows: 1fr 1fr;
}
.elevatorColumn {
  background-color: rgb(48, 203, 209);
  width: 80px;
  height: 100px;
  display: flex;
}
.elevatorColumn::before {
  content: "";
  display: block;
  width: 10px;
  height: 100%;
  border-left: 1.5px solid gray;
}

.floorsColumn {
}
.floor {
  margin-top: 25px;
  display: flex;
}
.callElevator {
  width: 15px;
  height: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 5px 0 0 10px;
  border: none;
  background-color: #fff;
  border: 0.5px solid;
  border-radius: 10%;
  color: rgb(48, 203, 209);
  cursor: pointer;
  transition: 0.3s all ease;
}
.callElevator:hover {
  color: rgb(220, 145, 46);
}

span {
  font-size: 12px;
}
</style>
