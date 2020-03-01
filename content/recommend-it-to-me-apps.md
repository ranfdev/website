+++
title = "Recommend it to me - apps"
date = 2019-12-10
+++

I want a world with **less advertising** and more user **recommendations from real people**.
I think it would be cool if everyone could put something like this in his blog,
to promote his favorite applications and projects.


## Example App listing

<style>
		.software-recommendations {
			display: grid;
			grid-template-columns: repeat(auto-fill, minmax(110px, 1fr));
			gap: 10px;
			font-size: 1rem
		}

		.recommendation-card {
			padding: 10px;
			background: #f0f0f0;
			border-radius: 10px;
			text-decoration: none;
		}

		.software-recommendations * {
			margin: 0;
		}
</style>
<div class="software-recommendations">
	<a class="recommendation-card" href="https://joinmastodon.org/">
			<img loading="lazy" src="https://raw.githubusercontent.com/tootsuite/mastodon/master/public/android-chrome-192x192.png">
			<h3>Mastodon</h3>
			<p>Social network</p>
	</a>
	<a class="recommendation-card" href="https://www.mozilla.org/en-US/firefox/new/">
			<img loading="lazy" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a0/Firefox_logo%2C_2019.svg/1200px-Firefox_logo%2C_2019.svg.png">
			<h3>Firefox</h3>
			<p>Web browser</p>
	</a>
	<a class="recommendation-card" href="https://neovim.io/">
			<img loading="lazy" src="https://avatars2.githubusercontent.com/u/6471485?s=200&v=4">
			<h3>Neovim</h3>
			<p>text editor</p>
	</a>
	<a class="recommendation-card" href="https://getaegis.app/">
			<img loading="lazy" src="https://getaegis.app/dist/images/icon.png">
			<h3>Aegis</h3>
			<p>2FA manager</p>
	</a>
	<a class="recommendation-card" href="https://about.riot.im/">
			<img loading="lazy" src="https://riot.im/app/welcome/images/logo.svg">
			<h3>Riot.im</h3>
			<p>Decentralized chats</p>
	</a>
	<a class="recommendation-card" href="https://meet.jit.si/">
		<img loading="lazy" src="https://raw.githubusercontent.com/jitsi/jitsi-meet/master/images/apple-touch-icon.png">
		<h3>Jitsi</h3>
		<p>P2P calls</p>
	</a>
	
</div>

### App listing code
```html
<style>
	.software-recommendations {
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(110px, 1fr));
		gap: 10px;
		font-size: 1rem
	}

	.recommendation-card {
		padding: 10px;
		background: #f0f0f0;
		border-radius: 10px;
		text-decoration: none;
	}

	.software-recommendations * {
		margin: 0;
	}
</style>

<div class="software-recommendations">
	<!-- start app item -->
	<a href="https://joinmastodon.org/">
		<img loading="lazy" src="https://raw.githubusercontent.com/tootsuite/mastodon/master/public/android-chrome-192x192.png">
		<h3>Mastodon</h3>
		<p>Social network</p>
	</a>
	<!-- end app item -->

	<!-- just copy the app item here how many times you want -->
</div>

```