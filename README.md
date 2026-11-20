function dailyLog234() {
  const journeys = [
    { route: "A", fare: 2.80 },
    { route: "B", fare: 3.20 },
    { route: "A", fare: 2.80 },
    { route: "C", fare: 3.50 },
    { route: "B", fare: 3.20 }
  ];

  const totalTrips = journeys.length;

  const totalCost = journeys.reduce(
    (sum, journey) => sum + journey.fare,
    0
  );

  const averageFare = totalCost / totalTrips;

  console.log("Daily Transport Report");
  console.log("----------------------");
  console.log(`Total Journeys: ${totalTrips}`);
  console.log(`Total Cost: €${totalCost.toFixed(2)}`);
  console.log(`Average Fare: €${averageFare.toFixed(2)}`);
}

dailyLog234();
