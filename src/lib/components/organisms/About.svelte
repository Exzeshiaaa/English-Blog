<script>
	import SparklingHighlight from '$lib/components/molecules/SparklingHighlight.svelte';
	import Socials from '$lib/components/molecules/Socials.svelte';
	import Image from '../atoms/Image.svelte';
</script>

<section id="about" style="text-align: justify;">
	<div class="info">
		<h2>
			Let's start by introducing the different paper topics in the
			<br />
			<SparklingHighlight color="secondary">BLOG INTRODUCTION!</SparklingHighlight>
		</h2>
		<p>
			Our society is rampant with complex issues that influence the lives of people. While some of
			these problems may not seem obvious, they manifest in several ways which include interactions,
			systems, culture, and even the media consumed by the people. In this blog, we present four
			papers that delve deeply into specific societal issues providing insights, knowledge, and
			suggestions that may contribute to the development of a better and prepared society.
		</p>
	</div>

	<div class="image">
		<Image src="/images/societal-image.png" alt="Sample for the static template" />
	</div>
</section>

<section id="about" style="text-align: justify;">
	<div class="info">
		<p>
			Starting off with “How Everything Changed: Colonization in Avatar: The Last Airbender” by
			<span style="font-weight: bold;">Crizanne Chanelle Mejica</span>, in the world of the animated
			series, there are people who can control one of the four elements: water, earth, fire, or air.
			There is balance between the four nations, each representing one for these elements. There was
			peace until the Fire Nation Attacked. Learn about how animated series portray the impacts of
			colonization in this analysis paper and discover how it serves as the common root of
			political, societal, and cultural challenges within its world.
		</p>

		<br />

		<p>
			Meanwhile, focusing on the domain of data security and privacy, the paper “Health Insurance or
			Information Liability: An Analysis Behind the PhilHealth Data Breach and its Implications” by
			<span style="font-weight: bold;">Adrian Perez</span> provides an extensive analysis behind the
			PhilHealth data breach, its implications, and the steps that were taken to respond to the incident.
			Data security is often ignored because of the low attention it gets from the communities in the
			Philippines. In this paper, he discusses current trends of how much the Philippines is being attacked
			through this method and how it goes unnoticed in news until a major incident blows up such as the
			PhilHealth Data Breach Incident.
		</p>
	</div>

	<div class="image">
		<Image src="/images/society.png" alt="Sample for the static template" />
	</div>
</section>

<div style="text-align: justify;">
	<p>
		Analyzing the Philippine culture, “Guardians Against Grooming: Protecting Filipino Children from
		Exploitation” by <span style="font-weight: bold;">Janinalaine Platero</span> emphasizes how grooming
		and pedophilia are alarmingly normalized in the Philippine society. The paper explores the characteristics
		and effects of grooming and pedophilia. Due to the manipulative and secretive background of these
		heinous acts, they are often difficult to detect, lurking unnoticed within our society.The cultural
		factors that contribute to the normalization grooming and pedophilia are also analyzed in this paper
		which will provide the readers with nuanced understanding on why this issue is rampant in the Philippines.
		This analysis paper does not only aim to raise awareness but also to advocate for collective action
		to protect the Filipino youth.
	</p>

	<br />

	<p>
		Finally, the paper “Unpacking the Toxic Alpha Male Mindset and its Societal Repercussions” by
		<span style="font-weight: bold;">Aaron Tolentino</span> shows the concept of the `alpha male` which
		has deeply influenced societal norms and gender roles, characterized by traits like dominance and
		aggression. Recently, social media has amplified this toxic culture, with figures like Andrew Tate
		promoting misogynistic ideologies. This paper critically examines the prevalence and impact of alpha
		male culture, focusing on its digital manifestations. By analyzing harmful stereotypes and power
		dynamics, we aim to highlight the terrible effects of toxic masculinity on progress and gender equality.
		Drawing from feminist theories, we explore the motivations behind this movement and its resistance
		to societal change.
	</p>

	<br />

	<p>
		Bringing up these societal complexities as a topic of discourse for the community not only
		allows other people to be aware of it but it also elevates and highlights the importance of not
		just knowing about it, but taking action against it as well. Through the use of this blog, our
		group aims to spread, educate, and place importance on these issues to demand a better program,
		system, and response from each sector of the society. We believe that taking action,
		hand-in-hand, with the government against these will elevate both the lifestyle of the people in
		the community and the basic rights they deserve to have.
	</p>

	<br />

	<div class="socials">
		<span>Socials:</span>
		<Socials />
	</div>
</div>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#about {
		position: relative;
		display: grid;
		grid-template-columns: 500px 250px;
		align-items: center;
		justify-content: space-between;
		padding-bottom: 50px;

		@include for-phone-only {
			grid-template-columns: 1fr;
			justify-items: center;
			gap: 20px;
		}

		.info {
			display: flex;
			flex-direction: column;
			gap: 10px;
			h2 {
				@include for-phone-only {
					text-align: center;
				}
			}

			p {
				@include for-phone-only {
					text-align: justify;
				}
			}

			@include for-phone-only {
				gap: 20px;
			}
		}

		.socials {
			display: flex;
			align-items: center;
			gap: 15px;

			@include for-phone-only {
				justify-content: center;
				margin-bottom: 10px;
				span {
					display: none;
				}
			}
		}

		.image {
			width: 220px;
			height: 220px;
		}
	}
</style>
