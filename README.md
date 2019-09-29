# JSL-Flex
Extremely lightweight (233 bytes minified and gzip) responsive mobile first grid system. Works in all modern browsers including IE 11.

## Easy to use
Place your content inside rows and columns with their width specified in 10 percent steps.

        <div class="row">
          <div class="col col-20"> col-20 </div>
          <div class="col col-30"> col-30 </div>
          <div class="col col-50"> col-50 </div>
        </div>

## Responsive
![Large](/images/large.png "Large Screen Size")  
Large Screen Size (Desktop Mode)

![Medium](/images/medium.png "Medium Screen Size")  
Medium Screen Size (Tablet Mode)

![Small](/images/small.png "Small Screen Size")  
Small Screen Size (Mobile Mode)

## Include it in your project
Copy the jsl-flex.css or jsl-flex.min.css file from this repo or simply copy the code into one of your css files. The whole grid system is only 446 charaters (minified).


		.row {
			display: flex;
			flex-wrap: wrap;
		}

		.col, .row {
			width: 100%;
			position: relative;
			box-sizing: border-box;
		}

		@media (min-width: 45em) {
			.col-40 { width: 80%; 
			flex-grow: 1; }
			.col-30 { width: 60%;
			flex-grow: 1; }
			.col-20 { width: 40%;
			flex-grow: 1; }
			.col-10 { width: 20%; 
			flex-grow: 1; }
		}

		@media (min-width: 70em) {
			.col-100 { width: 100% }
			.col-90 { width: 90% }
			.col-80 { width: 80% }
			.col-70 { width: 70% }
			.col-60 { width: 60% }
			.col-50 { width: 50% }
			.col-40 { width: 40% }
			.col-30 { width: 30% }
			.col-20 { width: 20% }
			.col-10 { width: 10% }
		}
