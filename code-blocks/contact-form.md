```jsx
function ContactForm() {
  const [formData, setFormData] = useState({ name: '', email: '', message: '' });
  const [errors, setErrors] = useState({});

  const handleSubmit = (e) => {
    e.preventDefault();
    // Validate
    if (!formData.email.includes('@')) {
      setErrors({ email: 'Invalid email' });
      return;
    }
    // Submit logic
    console.log('Form submitted:', formData);
  };

  return (
    <form onSubmit={handleSubmit}>
      <input 
        value={formData.name}
        onChange={(e) => setFormData({...formData, name: e.target.value})}
      />
      {errors.email && <p className="text-red-500">{errors.email}</p>}
      <button type="submit">Submit</button>
    </form>
  );
}
```