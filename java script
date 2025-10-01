document.getElementById('reviewForm').addEventListener('submit', function(e) {
  e.preventDefault();

  const name = document.getElementById('name').value.trim();
  const wine = document.getElementById('wine').value.trim();
  const rating = document.getElementById('rating').value;
  const comment = document.getElementById('comment').value.trim();

  if (!name || !wine || !rating || !comment) return;

  const reviewList = document.getElementById('reviewList');

  const card = document.createElement('div');
  card.className = 'review-card';
  card.innerHTML = `
    <h3>${wine} <small>(Rated: ${rating}/10)</small></h3>
    <p>${comment}</p>
    <p><em>— ${name}</em></p>
  `;

  reviewList.prepend(card); // add new review to top

  this.reset();
});
