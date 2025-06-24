//# js-practice
const players = [
  { name: "Arya", score: 150, level: 3 },
  { name: "Zoya", score: 180, level: 2 },
  { name: "L", score: 150, level: 2 },
  { name: "Karan", score: 120, level: 4 },
  { name: "Mira", score: 180, level: 3 },
];

const order = players.sort((a, b) => {
  if (a.score !== b.score) return b.score - a.score;
  else {
    return a.level - b.level;
  }
});
console.log(order);
order.forEach((player) => {
  console.log(`${player.name} (Level ${player.level}) - ${player.score} pts`);
});
