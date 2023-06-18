<template>
	<header class="header">
		<a href="#" class="logo">Tours</a>

		<nav class="navbar">
			<a href="#" class="active">Home</a>
			<a href="#">About</a>
			<a href="#">Portfolio</a>
			<a href="#">Services</a>
			<a href="#">Contact</a>
		</nav>
	</header>
</template>

<script setup></script>

<style lang="scss" scoped>
	.header {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		padding: 20px 100px;
		background: rgba(255, 255, 255, 0.1);
		display: flex;
		justify-content: space-between;
		align-items: center;
		backdrop-filter: blur(10px);
		border-bottom: 2px solid rgba(255, 255, 255, 0.2);

		.logo {
			color: #fff;
			font-size: 25px;
			text-decoration: none;
			font-weight: 500;
			cursor: default;
		}

		.navbar a {
			color: #fff;
			font: 18px;
			text-decoration: none;
			margin-left: 35px;
			transition: 0.3s;
		}

		.navbar a:hover,
		.navbar a.active {
			color: #f00;
		}
	}

	.header::before {
		content: "";
		position: absolute;
		top: 0;
		left: -100%;
		width: 100%;
		height: 100%;
		background: linear-gradient(
			90deg,
			transparent,
			rgba(255, 255, 255, 0.4),
			transparent
		);
		transition: 0.5s;
	}

	.header:hover::before {
		left: 100%;
	}
</style>
