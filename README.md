import React from 'react';

function SoftwareEngineer() {
  const name = "Neema";
  const role = "Software Engineer";
  const languageSpoken = ["Swahili", "English"];

  const sayHi = () => {
    console.log("Thanks for dropping by, hope you find some of my work interesting.");
  };

  const code = ["Javascript", "Reactjs", "HTML", "CSS", "Java", "Bootstrap"];
  const tools = ["Stack Overflow", "Node", "Styled-Components", "Github", "Music"];
  const techCommunities =
	{
    Manager: "My own management",
    "Building stuff": "Writing product code",
  };

  return (
    <div>
      <h1>{name}</h1>
      <p>Role: {role}</p>
      <p>Languages Spoken: {languageSpoken.join(", ")}</p>
      <button onClick={sayHi}>Say Hi</button>

      <h2>Skills:</h2>
      <ul>
        {code.map((language, index) => (
          <li key={index}>{language}</li>
        ))}
      </ul>

      <h2>Tools:</h2>
      <ul>
        {tools.map((tool, index) => (
          <li key={index}>{tool}</li>
        ))}
      </ul>

      <h2>Tech Communities:</h2>
      <ul>
        {Object.entries(techCommunities).map(([key, value]) => (
          <li key={key}>
            <strong>{key}:</strong> {value}
          </li>
        ))}
      </ul>
    </div>
  );
}

export default SoftwareEngineer;
