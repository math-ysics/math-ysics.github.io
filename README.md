/* Basic Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Times New Roman", Times, serif;
  color: #333;
  line-height: 1.6;
  padding: 20px;
  background-color: #f4f4f9;
}

header, main {
  margin: 20px;
}

h1, h2 {
  font-weight: bold;
  color: #0056b3; /* A deeper shade of blue for better readability */
}

h1 {
  font-size: 32px;
  margin-bottom: 10px;
}

h2 {
  font-size: 24px;
  margin-top: 20px;
  margin-bottom: 5px;
}

p {
  font-size: 18px;
  font-style: italic;
  color: #555;
  margin-bottom: 10px;
}

a {
  color: #d6336c; /* A vibrant shade of pink for links to stand out */
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

img {
  max-width: 100%;
  height: auto;
  border-radius: 8px; /* Slightly rounded corners for images */
}

/* Flex container for images */
div[style*="flex"] {
  display: flex;
  gap: 10px; /* Adds space between the flex items */
  justify-content: center; /* Center-aligns flex items */
  flex-wrap: wrap; /* Enables wrapping of items */
}

/* Specific adjustments for smaller screens */
@media (max-width: 768px) {
  h1 {
    font-size: 28px;
  }

  h2 {
    font-size: 22px;
  }

  p {
    font-size: 16px;
  }
}
