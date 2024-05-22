<script>
	import heroBanner from '$lib/images/hero-image.jpg';
	//   import "./app.css";

    function copyToClipboard(text) {
    navigator.clipboard.writeText(text).then(() => {
      alert('Copied to clipboard');
    }).catch(err => {
      console.error('Failed to copy: ', err);
    });
  }
</script>

<div class="landing container-sm">
	<div class="hero">
		<div class="heroText">
			<div class="title">
				<h1>Revolutionize Your Web Development with Our <span>SveltyCMS</span></h1>
				<h2>
					The ultimate backend dashboard combining the best features from leading CMS platforms.
				</h2>

                <pre style="position:relative;"><code class="language-bash">npx create-sveltekit-cms my-project</code> <button class="absolute top-2 right-2" on:click={() => copyToClipboard('npx create-sveltekit-cms my-project\ncd my-project\nnpm install\nnpm run dev')}><i class="fa-regular fa-clipboard"></i></button></pre>
			</div>
			<div class="cta">
				<a class="cta1" href="">Get Started</a>
				<a class="cta2" href="#anchor">Learn More</a>
			</div>
		</div>

		<div class="thumb">
			<img src={heroBanner} alt="" />
		</div>
	</div>
	<div class="features py-6">
        <div class="titleBox">
            <h2 class="orange">	Build apps fast.</h2>

            <p>
            
Get your backend done in minutes instead of weeks.
Easily build customizable content API and use them with a modern tech stack.
            </p>
        </div>
		<div class="myGrid" id="anchor">
			
				
		
	
				<div class="fBox">
					<i class="fa-solid fa-code"></i>

					<h3>Open Source</h3>
					<p>
                        Forever. The entire codebase is available on GitHub and maintained.</p>
				</div>
				<div class="fBox">
					<i class="fa-solid fa-upload"></i>

					<h3>Flexible Media Uploading</h3>
					<p>Easily upload and manage your media files with our intuitive interface.</p>
				</div>
				<div class="fBox">
					<i class="fa-solid fa-brush"></i>
					<h3>User-Friendly Icon GUI</h3>
					<p>Navigate effortlessly with our easy-to-understand icon-based GUI.</p>
				</div>
	
			
				<div class="fBox">
					<i class="fa-solid fa-sitemap"></i>
					<h3>Custom Collections</h3>
					<p>Define and display collections and tables with unmatched flexibility.</p>
				</div>
	
			
				<div class="fBox">
					<i class="fa-solid fa-shield-halved"></i>
					<h3>High & Flexible Security</h3>
					<p>Secure your data with our robust and customizable security features.</p>
				</div>

			
				<div class="fBox">
					<i class="fa-solid fa-image"></i>
					<h3>Image Editor</h3>
					<p>Edit images on the fly with our integrated image editor.</p>
				</div>
            </div>
		</div>
	</div>


<style>
	.orange {
		color: #ff3e00;
	}
	.py-6 {
		padding-block: 7em;
	}

	p {
		font-size: 1em;
		line-height: 1.4em;
	}
	h2 {
		font-size: clamp(1.5rem, 2vw, 2rem);
		line-height: 1.1em;
		margin-bottom: 14px;
	}

	h3 {
		font-size: 22px;
		line-height: 1.2em;
		margin-bottom: 0.5em;
	}

	.landing {
        padding-inline: 1em;
        width: 1140px;
        max-width: 100%;
		margin-top: 7em;
		position: absolute;
		left: 50%;
		transform: translateX(-50%);
	}
	.hero {
		text-align: center;
	}
	.heroText {
		max-width: 992px;
		margin-inline: auto;
	}
	.hero h1 {
		font-size: clamp(1.5rem, 5vw, 3rem);
		line-height: 1.1em;
		margin-bottom: 0.5em;
	}
	.hero h1 span {
		color: #ff3e00;
	}
	.hero h2 {
		font-size: clamp(1em, 0.5vw, 1.5em);
		line-height: 1.2em;
		font-weight: 400;
		margin-bottom: 1.5em;
	}
	.hero .cta {
		margin-bottom: 3em;
		display: flex;
		justify-content: center;
		gap: 1em;
	}

	.hero .cta a {
		padding: 10px 30px;
		border: 1.5px solid #ff3e00;
		border-radius: 30px;
	}

	.hero .cta .cta1 {
		background: #ff3e00;
		color: #ffffff;
	}

    .hero pre{
        display: inline-block;
    padding: 7px 24px;
    border: 1px solid #000000;
    border-radius: 16px;
    background: #eeeeee;
    /* color: #ffffff; */
    margin-bottom: 2em;
}

.hero pre i{
    color: #ff3e00;
}
    

    .titleBox{
        text-align: center;
        max-width: 660px;
    margin-bottom: 2.5em;
    margin-inline: auto;
    }

    .myGrid{
        
        display: grid;
        grid-template-columns: repeat( auto-fit, minmax(270px, 1fr) );
        gap: 1.5em;
    }

	.fBox {
		padding: 1em 2em 2em 1em;
		border: 1px solid #eeeeee;
		border-radius: 20px;
	}

	.fBox i {
		color: #ff3e00;
		/* background: #ff3e00; */
		font-size: 1em;
		margin-bottom: 1em;
		width: 40px;
		height: 40px;
		/* background: #eeeeee; */
		text-align: center;
		line-height: 40px;
		border: 1px solid;
		border-radius: 7px;
	}
</style>
