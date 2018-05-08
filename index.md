---
layout: default
---

<!-- FEATURE Section-->
<section>

	<header class="major">
		<h2>Features</h2>
	</header>

	<div class="features">

		<article>
			<span class="icon fa-diamond"></span>
			<div class="content">
				<h3>Commons</h3>
				<p>I beni comuni sono quei beni condivisi da una comunità. Il termine è legato al concetto di condivisione e comunione e lo si ritrova anche all'interno della moderna cultura digitale ed informatica. Sono beni di tutti da difendere e diffondere.</p>
			</div>
		</article>


		<article>
			<span class="icon fa-paper-plane"></span>
			<div class="content">
				<h3>Condivisione</h3>
				<p><i>"Chi ricava un'idea da me, ricava conoscenza senza diminuire la mia: come chi accende la sua condela con la mia riceve luce senza lasciarmi al buio."</i> - Thomas Jefferson - <br/> Il sapere è di tutti e la conoscenza nasce sempre dalla condivisione.</p>
			</div>
		</article>


		<article>
			<span class="icon fa-rocket"></span>
			<div class="content">
				<h3>Le 4 liberta</h3>
				<p>Il “Software libero” è software che rispetta <b>la libertà</b> degli utenti e la comunità.<br/> Un programma è software libero se gli utenti del programma godono delle quattro libertà fondamentali: <b>eseguire</b>, <b>studiare</b>, <b>ridistribuire</b> e <b>migliorare</b>.
				<!--<br/><ul>
					<li>Libertà di <b>eseguire</b> il programma come si desidera, per qualsiasi scopo (libertà 0).</li>
					<li>Libertà di <b>studiare</b> come funziona il programma e di modificarlo in modo da adattarlo alle proprie necessità (libertà 1). L'accesso al codice sorgente ne è un prerequisito.</li>
					<li>Libertà di <b>ridistribuire</b> copie in modo da aiutare il prossimo (libertà 2).</li>
					<li>Libertà di <b>migliorare</b> il programma e distribuirne pubblicamente i miglioramenti da voi apportati (e le vostre versioni modificate in genere), in modo tale che tutta la comunità ne tragga beneficio (libertà 3). L'accesso al codice sorgente ne è un prerequisito.</li>
					</ul>-->
				</p>
			</div>
		</article>


		<article>
			<span class="icon fa-signal"></span>
			<div class="content">
				<h3>Cittadinanza digitale</h3>
				<p>L'uso critico della rete e degli strumenti digitali e informatici permette di agire consapevolmente nel mondo moderno. Il software libero favorisce lo sviluppo di utilizzi virtuosi della tecnologia in virtù della sua qualità di trasparenza e rispetto delle libertà individuali dei suoi utilizzatori. Saper agire in maniera competente nel mondo complesso contemporaneo non è più solo un'opzione, ma diventa necessità per proteggere i beni (fisici e intellettuali) di tutti.</p>
			</div>
		</article>

	</div>
</section>




<!-- POSTS Section -->
<section>
	<header class="major">
		<h2>Posts</h2>
	</header>
	<div class="posts">

	{% for post in site.posts%}

	<article>
		<a href="{{site.baseurl}}{{post.url}}" class="image"><img src="assets/images/{{post.image}}" alt="" /></a>
		<h3><a href="{{site.baseurl}}{{post.url}}">{{ post.title }}</a></h3>
		{{ post.excerpt}}
		<ul class="actions">
			<li><a href="{{site.baseurl}}{{post.url}}" class="button">More</a></li>
		</ul>
	</article>

	{% endfor %}


	<!--
		<article>
			<a href="#" class="image"><img src="assets/images/pic01.jpg" alt="" /></a>
			<h3>Interdum aenean</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>



		<article>
			<a href="#" class="image"><img src="assets/images/pic02.jpg" alt="" /></a>
			<h3>Nulla amet dolore</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>



		<article>
			<a href="#" class="image"><img src="assets/images/pic03.jpg" alt="" /></a>
			<h3>Tempus ullamcorper</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>



		<article>
			<a href="#" class="image"><img src="assets/images/pic04.jpg" alt="" /></a>
			<h3>Sed etiam facilis</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>



		<article>
			<a href="#" class="image"><img src="assets/images/pic05.jpg" alt="" /></a>
			<h3>Feugiat lorem aenean</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>



		<article>
			<a href="#" class="image"><img src="assets/images/pic06.jpg" alt="" /></a>
			<h3>Amet varius aliquam</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>
-->


	</div>
</section>
