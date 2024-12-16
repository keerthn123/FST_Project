http://127.0.0.1:9000/api/get-workout/
Request: body{
  "goal":"body building",
  "level":"extreme hard"
}
[
  {
    "name": "Push-ups",
    "sets": "3",
    "reps": "10-15",
    "benifits": "Improves chest, shoulder, and triceps strength; builds upper body endurance."
  },
  {
    "name": "Squats",
    "sets": "3",
    "reps": "10-15",
    "benifits": "Strengthens legs and glutes; improves lower body power and stability."
  },
  {
    "name": "Walking Lunges",
    "sets": "3",
    "reps": "10-12 per leg",
    "benifits": "Builds leg and glute strength; improves balance and coordination."
  }
]

#=============================================================

http://127.0.0.1:9000/api/get-meals/
Request: body{
  "mealType":"Breakfast",
  "targetCals":"2000"
}
{
  "meals": [
    {
      "name": "Oatmeal with Berries and Nuts",
      "quantity": "300 grams",
      "imageUrl": "https://example.com/oatmeal.jpg",
      "benefits": "Provides complex carbohydrates for sustained energy, fiber for digestion, antioxidants from berries, and healthy fats from nuts."
    },
    {
      "name": "Scrambled Eggs with Avocado Toast and Smoked Salmon",
      "quantity": "500 grams",
      "imageUrl": "https://example.com/eggs_avocado.jpg",
      "benefits": "Excellent source of protein, healthy fats from avocado and salmon, and essential vitamins and minerals."
    }
  ]
}

#===========================================================

http://127.0.0.1:9000/api/get-cals/

Request: body {
  "meal":"Burger",
  "quantity":"200 grams"
}

{
  "caloryCount": "500",
  "contains": "The given food contains proteins, fats, carbohydrates, sodium, and some vitamins and minerals. The exact nutritional content varies depending on the specific ingredients and preparation method of the burger.",
  "suggestions": "A 200g burger provides approximately 500 calories.  This is a moderate calorie intake. To maintain a balanced diet, consider incorporating more fruits, vegetables, and whole grains throughout the day.  A brisk 30-minute walk would be a good way to help balance your calorie intake today.",
  "imageUrl": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSK6ghC4OB1yk7uqJoEupPCdoFFfYecE5J_UQ&s"
}