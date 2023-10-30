<template>
    <div class="timers">
      <h3>
        Time Between Meals
      </h3>
      <div class="timer-container">
        <div class="timer">
          {{ hoursDisplay }}:{{ minutesDisplay }}:{{ secondsDisplay }}
        </div>
        <button @click="startTimer" :disabled="isTimerRunning">Start</button>
        <button @click="stopTimer" :disabled="!isTimerRunning">Stop</button>
        <button @click="resetTimer" :disabled="isTimerRunning">Reset</button>
      </div>

    </div>
  </template>      
  
  <script>
  export default {
    name: 'TimersView',
    data() {
      return {
        hours: 0,
        minutes: 0,
        seconds: 0,
        isTimerRunning: false,
        timerInterval: null,
      };
    },
    computed: {
      hoursDisplay() {
        return this.padZero(this.hours);
      },
      minutesDisplay() {
        return this.padZero(this.minutes);
      },
      secondsDisplay() {
        return this.padZero(this.seconds);
      },
    },
    methods: {
      padZero(value) {
        return value.toString().padStart(2, '0');
      },
      startTimer() {
        if (!this.isTimerRunning) {
          this.isTimerRunning = true;
          this.timerInterval = setInterval(() => {
            this.seconds++;
  
            if (this.seconds === 60) {
              this.seconds = 0;
              this.minutes++;
  
              if (this.minutes === 60) {
                this.minutes = 0;
                this.hours++;
              }
            }
          }, 1000);
        }
      },
      stopTimer() {
        if (this.isTimerRunning) {
          this.isTimerRunning = false;
          clearInterval(this.timerInterval);
        }
      },
      resetTimer() {
        this.isTimerRunning = false;
        clearInterval(this.timerInterval);
        this.hours = 0;
        this.minutes = 0;
        this.seconds = 0;
      },
    },
    beforeUnmount() {
      if (this.timerInterval) {
        clearInterval(this.timerInterval);
      }
    },
  };
  </script>
  
  <style scoped lang="scss">
 *{
    margin: 0;
    padding: 0;
    background-color: #151515;
    border-radius: 5px;

    h3{
      text-align: center;
      margin-top: 10px;
      padding-top: 10px;
    }

    .timer-container {
    text-align: center;
    margin-top: 10px;
    padding-top: 20px;
    padding-bottom: 20px;
  }
  
  .timer-container .timer {
    font-size: 36px;
    font-weight: bold;
    margin-bottom: 10px;
  }
  
  .timer-container button {
    padding: 10px 20px;
    background-color: #8B0000;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
  }
  
  .timer-container button:disabled {
    background-color: #ccc;
    cursor: not-allowed;
  }
 }


 
  </style>
  