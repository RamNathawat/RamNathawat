# Hi there! 👋 I'm Ram Nathawat

Add a waving animation to your introduction using CSS. This simple CSS class adds a waving effect to the text when hovered over.

## Waving Animation

Copy the following CSS code into your project:

```css
.span .wave {
  animation-name: wave-animation;  /* Name of @keyframes element below */
  animation-duration: .75s;  /* Wave speed */
  animation-iteration-count: infinite;
  animation-timing-function: linear;
  animation-play-state: paused;
  transform-origin: 70% 70%;  /* Pivot from bottom-left palm */
  display: inline-block;
  font-size: 8rem;
}

.span .wave:hover {
  animation-play-state: running; /* Play animation on mouse hover */
}

@keyframes wave-animation {
  0% { transform: rotate( 0deg ) }
  25% { transform: rotate( -10deg ) }
  75% { transform: rotate( 12deg ) }
  100% { transform: rotate( 0deg ) }
}

<span class="wave">Hi 👋, I'm Ram Nathawat</span>
