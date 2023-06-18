<template>
	<footer class="footer">
		<p>
			<span class="developer">Developer: </span
			><a href="https://github.com/Montcat" class="developer-link">Mont King</a>
		</p>
		<p>
			<span class="reference">Reference: </span
			><a href="https://www.youtube.com/@codehal">Codehal</a>
		</p>
	</footer>
</template>

<script setup></script>

<style lang="scss" scoped>
	.footer {
		position: fixed;
		bottom: 0;
		left: 0;
		width: 100%;
		padding: 20px 100px;
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 2rem;

		p {
			color: #fff;
			font-size: 18px;

			a {
				text-decoration: none;
				color: #ff0000d1;
			}
		}
	}
</style>
