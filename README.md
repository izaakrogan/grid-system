This is a ######tiny grid system for my own use.

If you want to give it a whirl, grid elements are given a class starting with 'grid'

You might want to stick those elements in the grid-container, with your html might looking something like this:


<div class="grid-container">
	<div class="grid">
		<p>I start on the left</p>
	</div>
	<div class="grid">
		<p>I start in the middle</p>
	</div>
	<div class="grid">	
		<p>I start on the right</p>
	</div>
</div>

You will need to add your own 'grid' classes and breakpoints. For example:

@media (min-width: 1000px) {
	.grid-1 {
		width: 33.333333%;
	}
}

@media (max-width: 1000px) {
	.grid-1 {
		width: 50%;
	}
}

@media (max-width: 400px) {
	.grid-1 {
		width: 100%;
	}
}