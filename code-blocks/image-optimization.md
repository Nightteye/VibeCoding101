```jsx
// Optimized image
<img 
  src="/images/hero.webp" 
  alt="Hero image"
  loading="lazy"
  className="w-full h-auto"
/>

// Responsive image
<img 
  srcset="/images/small.webp 480w, /images/large.webp 1080w"
  sizes="(max-width: 768px) 480px, 1080px"
  src="/images/large.webp"
  alt="Responsive"
/>
```
