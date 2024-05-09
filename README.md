- 👋 Hi, I’m @Rahulofficial7050
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Rahulofficial7050/Rahulofficial7050 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Repository Status</title>
</head>
<body>
    <h1>GitHub Repository Status</h1>
    <div id="status"></div>

    <script>
        // Make a request to GitHub API to fetch repository status
        fetch('https://api.github.com/repos/Pandeycoder/your-repo')
            .then(response => response.json())
            .then(data => {
                // Display repository status
                document.getElementById('status').innerHTML = `
                    <h2>Repository Status</h2>
                    <p>Repository Name: ${data.name}</p>
                    <p>Open Issues: ${data.open_issues_count}</p>
                    <p>Watchers: ${data.watchers_count}</p>
                    <p>Stars: ${data.stargazers_count}</p>
                `;
            })
            .catch(error => console.error('Error fetching data:', error));
    </script>
</body>
</html>
