<template>
    <section>
        <div id="ffmi">
            <h2>Fat Free Mass Index</h2>
            <h3>FFMI allows us to take into account a person's bodyfat %. </h3>
            <h3>How is FFMI diffrent from BMI?</h3>
            <h4>Lets look at the BMI of Arnold Schwetzinger at his peak physique. </h4>
            <ul>
                <li>{{Arnold}}</li>
            </ul>
            <h3>Even when we use Arnolds Stage weight of 235lbs he would be considered Obese with a BMI of around 30.2
                <img src="http://www.institutefornaturalhealing.com/wp-content/uploads/2016/02/arnold-bmi-393x314.jpg" alt="">
            </h3>
            <h3>Kinda funny how one of the most popular ways to monitor health is actually really bad at accurtley determaining
                someones fitness level</h3>
        </div>


        <div id="ffmiCalc">
            <div id="height">
                <li>
                    <label for="HeightFT">Height FT</label>
                    <input v-model="HeightFT">

                </li>
                <li>
                    <label for="HeightIN">Height In</label>
                    <input v-model="HeightIN">
                </li>
            </div>
            <li>
                <label for="Bodyfat">Bodyfat %</label>
                <input v-model="Bodyfat">
            </li>
            <li>
                <label for="Weight">Weight</label>
                <input v-model="Weight">
            </li>
            <h3>FFMI Score: {{ FFMI }} </h3>
        </div>


    </section>
</template>
<script>
    export default {
        data() {
            return {
                HeightFT: '',
                HeightIN: '',
                Bodyfat: '',
                Weight: '',
                FFMI: '',
                Arnold: {
                    Height: 6.2,
                    contestWeight: 235,
                    offSeasonWeight: 260,
                    Arms: 22,
                    Chest: 57,
                    Waist: 34,
                    Thighs: 28.5,
                    Calves: 20,
                }
            }
        },
        computed: {

            leanWeight: function () {
                return (this.Weight * (1 - (this.Bodyfat / 100)))
            },
            height: function () {
                return (((this.HeightFT * 12) + (this.HeightIN)) * Math.sqrt(.0254))
            }
             },
             FFMI: function () {
            return ((this.leanWeight / 2.2) / this.height)
             }
    }
</script>
<style>
    #ffmi {
        color: white;
    }

    #ffmiCalc {
        color: white;
    }
</style>