```jsx 
function DataComponent() {
  const [loading, setLoading] = useState(true);
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch('/api/data')
      .then(res => res.json())
      .then(data => {
        setData(data);
        setLoading(false);
      });
  }, []);

  if (loading) {
    return <div className="animate-spin">Loading...</div>;
  }

  return <div>{data.title}</div>;
}

// Submit button state
<button 
  disabled={isSubmitting}
  className={isSubmitting ? 'opacity-50 cursor-not-allowed' : ''}
>
  {isSubmitting ? 'Submitting...' : 'Submit'}
</button>
```