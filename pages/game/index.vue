<template>
  <v-row
    justify="center"
    align="center"
    class="ma-0"
  >
    <v-col cols="12" sm="8" md="6">
      <v-stepper
        v-model="e13"
        vertical
        class="pb-4"
      >
        <v-stepper-header
          class="mb-4"
        >
          <v-card-title
            class="justify-space-between"
          >
            <span>Choose tornado!</span>
            <span>Score: {{ count }}</span>
          </v-card-title>
        </v-stepper-header>

        <v-stepper-step
          :complete="e13 > 1"
          step="1"
          class="pa-2"
        >
          Round
        </v-stepper-step>

        <v-stepper-content step="1">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <div>
                  <img
                    width="100"
                    height="70"
                    src="images/tornado/1.png"
                    alt="Tornado 1"
                    class="game-img"
                    @click="stepOne()"
                  >
                </div>
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/1.png"
                  alt="Element 1"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/2.png"
                  alt="Element 2"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

        <v-stepper-step
          :complete="e13 > 2"
          step="2"
          class="pa-2"
        >
          Round
        </v-stepper-step>

        <v-stepper-content step="2">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/3.png"
                  alt="Element 3"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/2.png"
                  alt="Tornado 2"
                  class="game-img"
                  @click="stepTwo()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/4.png"
                  alt="Element 4"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 3"
          step="3"
          class="pa-2"
         >
           Round
         </v-stepper-step>

        <v-stepper-content step="3">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/5.png"
                  alt="Element 5"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/6.png"
                  alt="Element 6"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/3.png"
                  alt="Tornado 3"
                  class="game-img"
                  @click="stepThree()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 4"
          step="4"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="4">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/7.png"
                  alt="Element 7"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/4.png"
                  alt="Tornado 4"
                  class="game-img"
                  @click="stepFour()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/8.png"
                  alt="Element 8"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 5"
          step="5"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="5">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/5.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="stepFive()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/9.png"
                  alt="Element 9"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/10.png"
                  alt="Element 10"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 6"
          step="6"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="6">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/11.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/12.png"
                  alt="Element 9"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/6.png"
                  alt="Element 10"
                  class="game-img"
                  @click="stepSix()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 7"
          step="7"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="7">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/13.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/14.png"
                  alt="Element 9"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/7.png"
                  alt="Element 10"
                  class="game-img"
                  @click="stepSeven()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 8"
          step="8"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="8">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/15.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/8.png"
                  alt="Element 9"
                  class="game-img"
                  @click="stepEight()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/16.png"
                  alt="Element 10"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

         <v-stepper-step
          :complete="e13 > 9"
          step="9"
          class="pa-2"
        >
           Round
        </v-stepper-step>

        <v-stepper-content step="9">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/17.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/18.png"
                  alt="Element 9"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/9.png"
                  alt="Element 10"
                  class="game-img"
                  @click="stepNine()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

        <v-stepper-step
          step="10"
          class="pa-2"
        >
          Round
        </v-stepper-step>

        <v-stepper-content step="10">
          <v-container
            class="pa-0"
            fluid
          >
            <v-row>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/tornado/10.png"
                  alt="Tornado 5"
                  class="game-img"
                  @click="openDialogWin()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/19.png"
                  alt="Element 9"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
              <v-col
                cols="sm"
                class="pa-2"
              >
                <img
                  width="100"
                  height="70"
                  src="images/element/20.png"
                  alt="Element 10"
                  class="game-img"
                  @click="openDialogDefeat()"
                >
              </v-col>
            </v-row>
          </v-container>
        </v-stepper-content>

      </v-stepper>
    </v-col>
    <v-dialog
      v-model="dialogWin"
      width="360"
    >
      <v-card>
        <v-card-title
          class="justify-center"
        >
          You won!
        </v-card-title>
        <v-card-text
          class="d-flex justify-center pb-0"
        >
          Your score: {{ count }}
        </v-card-text>
        <v-card-actions
          class="justify-center"
        >
          <v-btn
            text
            @click="newGame()"
          >
            New game
          </v-btn>
          <v-btn
            text
            @click="exitGame()"
          >
            Exit
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
    <v-dialog
      v-model="dialogDefeat"
      width="360"
    >
      <v-card>
        <v-card-title
          class="justify-center"
        >
          You lose
        </v-card-title>

        <v-card-actions
          class="justify-center"
        >
          <v-btn
            text
            @click="restartGame()"
          >
            Restart
          </v-btn>
          <v-btn
            text
            @click="exitDefeat()"
          >
            Exit
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </v-row>
</template>

<script>
export default {
  name: "GamePage",
  data() {
    return {
      e13: 1,
      dialogWin: false,
      dialogDefeat: false,
      count: ''
    }
  },
  methods: {
    openDialogWin() {
      this.dialogWin = true
      this.count = 100
    },
    openDialogDefeat() {
      this.dialogDefeat = true
    },
    newGame() {
      this.dialogWin = false
      this.$router.push('/');
    },
    exitGame() {
      this.dialogWin = false
      this.$router.push('/');
    },
    restartGame() {
      this.dialogDefeat = false
      this.$router.push('/');
    },
    exitDefeat() {
      this.dialogDefeat = false
      this.$router.push('/');
    },
    stepOne() {
      this.e13 = 2
      this.count = 10
    },
    stepTwo() {
      this.e13 = 3
      this.count = 20
    },
    stepThree() {
      this.e13 = 4
      this.count = 30
    },
    stepFour() {
      this.e13 = 5
      this.count = 40
    },
    stepFive() {
      this.e13 = 6
      this.count = 50
    },
    stepSix() {
      this.e13 = 7
      this.count = 60
    },
    stepSeven() {
      this.e13 = 8
      this.count = 70
    },
    stepEight() {
      this.e13 = 9
      this.count = 80
    },
    stepNine() {
      this.e13 = 10
      this.count = 90
    }
  }
}
</script>

<style>

  .game-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 5px;
    display: block;
  }

</style>
