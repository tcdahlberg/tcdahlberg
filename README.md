<style>
#githubProfile * {
  box-sizing: border-box;
}

#githubProfile {
  display: grid;
  grid-template-columns: repeat(12, [col-start] 1fr);
  gap: 20px;
}

/* Mobile first */
#githubProfile > * {
  border: 1px solid green;
  padding: 10px;
  grid-column: col-start / span 12;
}

@media (min-width: 576px) {
  #githubProfile .sidebar {
    grid-column: col-start / span 3;
  }
  #githubProfile .content, #githubProfile .footer {
    grid-column: col-start / span 9;
  }
}

@media (min-width: 768px) {
  #githubProfile .content {
    grid-column: col-start / span 9;
    grid-row: 2 / 4;
  }
  #githubProfile .sidebar {
    grid-column: col-start 10 / span 3;
  }
  #githubProfile .footer {
    grid-column: col-start / span 12;
  }
}
</style>

<div id="githubProfile">
<header class="head">### Hi there 👋!</header>
<div class="content">
- I'm a Principal Software Engineer at the <a href="https://stthomas.edu">Unveristy of St. Thomas</a> in Minnesota
- The lead developer for the Salesforce native event registration solution the <a href="https://sfdo-community-sprints.github.io/summit-events-app-documentation/">Summit Events App</a>
- 🐘 <a rel="me" href="https://mastodon.world/@tcdahlberg">Mastodon</a>
- 🔗 <a href="https://www.linkedin.com/in/thaddaeus/">LinkedIn</a>
- ☁️ <a href="https://trailblazer.me/id/tdahlberg">Salesforce Trailblazer Community</a>
- 🦋 <a href="https://bsky.app/profile/tcdahlberg.bsky.social">@tcdahlberg.bsky.social</a>
</div>
 <div class="sidebar">Sidebar</div>
  <footer class="footer">The footer</footer> 
</div>
