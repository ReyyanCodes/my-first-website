 <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Fit Hub</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background: #f4f7f6;
    color: #222;
}

header {
    background: #111;
    color: white;
    padding: 20px;
    text-align: center;
}

header h1 {
    font-size: 35px;
}

header p {
    margin-top: 8px;
    color: #ccc;
}

.hero {
    padding: 60px 20px;
    text-align: center;
    background: linear-gradient(135deg, #111, #333);
    color: white;
}

.hero h2 {
    font-size: 40px;
    margin-bottom: 15px;
}

.hero p {
    font-size: 18px;
    margin-bottom: 25px;
}

.btn {
    display: inline-block;
    background: #00c853;
    color: white;
    padding: 14px 25px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: bold;
}

.container {
    max-width: 1000px;
    margin: auto;
    padding: 40px 20px;
}

.section-title {
    text-align: center;
    font-size: 30px;
    margin-bottom: 30px;
}

.cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

.card {
    background: white;
    padding: 25px;
    text-align: center;
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
}

.card .icon {
    font-size: 45px;
    margin-bottom: 15px;
}

.card h3 {
    margin-bottom: 10px;
}

.card p {
    color: #666;
    line-height: 1.5;
}

.workout {
    margin-top: 50px;
}

.workout-box {
    background: white;
    padding: 25px;
    border-radius: 15px;
    margin-bottom: 15px;
    box-shadow: 0 3px 15px rgba(0,0,0,0.08);
}

.workout-box h3 {
    color: #00a844;
    margin-bottom: 8px;
}

footer {
    background: #111;
    color: white;
    text-align: center;
    padding: 25px;
    margin-top: 40px;
}

@media(max-width: 700px) {
    .cards {
        grid-template-columns: 1fr;
    }

    .hero h2 {
        font-size: 30px;
    }
}
</style>
</head>

<body>

<header>
    <h1>💪 FIT HUB</h1>
    <p>Your Fitness Journey Starts Here</p>
</header>

<section class="hero">
    <h2>Build a Stronger You</h2>
    <p>Train smart. Stay healthy. Become your best version.</p>

    <a href="#workouts" class="btn">Explore Workouts</a>
</section>

<div class="container">

    <h2 class="section-title">What We Offer</h2>

    <div class="cards">

        <div class="card">
            <div class="icon">🏋️</div>
            <h3>Strength Training</h3>
            <p>
                Improve your strength with simple and effective
                exercises.
            </p>
        </div>

        <div class="card">
            <div class="icon">🏃</div>
            <h3>Cardio</h3>
            <p>
                Improve your fitness with running, walking and
                other healthy activities.
            </p>
        </div>

        <div class="card">
            <div class="icon">🥗</div>
            <h3>Healthy Lifestyle</h3>
            <p>
                Learn healthy habits and make better everyday
                choices.
            </p>
        </div>

    </div>


    <section class="workout" id="workouts">

        <h2 class="section-title">Workout Ideas</h2>

        <div class="workout-box">
            <h3>🏃 Beginner Workout</h3>
            <p>
                Walking, light jogging, stretching and basic
                bodyweight exercises.
            </p>
        </div>

        <div class="workout-box">
            <h3>💪 Strength Workout</h3>
            <p>
                Squats, push-ups, lunges and other safe
                bodyweight exercises.
            </p>
        </div>

        <div class="workout-box">
            <h3>🧘 Flexibility</h3>
            <p>
                Gentle stretching and mobility exercises to
                improve movement.
            </p>
        </div>

    </section>

</div>

<footer>
    <p>© 2026 Fit Hub | Stay Active • Stay Healthy</p>
</footer>

<script>
document.querySelector(".btn").addEventListener("click", function() {
    alert("Welcome to Fit Hub! 💪");
});
</script>

</body>
</html>