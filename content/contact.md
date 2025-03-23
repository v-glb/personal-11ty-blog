---js
const eleventyNavigation = {
	key: "Kontakt",
	order: 4
};
---
# Kontaktiere mich

<p>Wenn du mir eine Nachricht schreiben willst, kannst du das gerne per E-Mail tun: <span id="email"></span></p>

<script>
	// JS obfucation to prevent spam bots from scraping
	document.addEventListener('DOMContentLoaded', function() {
		var user = 'v.networks';
		var domain = 'posteo.de';
		var email = user + '@' + domain;
		document.getElementById('email').innerHTML = '<a href="mailto:' + email + '">' + email + '</a>';
	});
</script>