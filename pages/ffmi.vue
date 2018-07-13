<template>
    <div>
        <h2>Fat Free Mass Index</h2>
        <h3>FFMI allows us to take into account a person's bodyfat %. </h3>
        <h3>So whats wrong with BMI</h3>
        <h4>Lets look at the BMI of Arnold Schwetzinger at his peak physique. </h4>
        <ul >
            <li>{{Arnold}}</li>  
        </ul>
        <h3>Even when we use Arnolds Stage weight of 235lbs he would be considered Obese with a BMI of around 30.2 <img src="http://www.institutefornaturalhealing.com/wp-content/uploads/2016/02/arnold-bmi-393x314.jpg" alt=""></h3>
        <h3>Kinda funny how one of the most popular ways to monitor health is actually really bad at accurtley determaining someones fitness level</h3>
    </div>
</template>
<script>
    export default {
        data() {
            return {
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
        }

    }
</script>
<style>
</style>