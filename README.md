<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>THughes 3D | Professional Printing Services</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #4f46e5;
            --primary-hover: #4338ca;
            --bg-dark: #0f172a;
            --card-bg: #1e293b;
            --text-main: #f8fafc;
            --text-dim: #94a3b8;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-dark);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* --- Hero Section --- */
        header {
            height: 80vh;
            background: linear-gradient(rgba(15, 23, 42, 0.7), rgba(15, 23, 42, 0.9)), 
                        url('https://images.unsplash.com/photo-1581092160607-ee22621dd758?auto=format&fit=crop&q=80&w=2070') center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
        }

        header h1 { font-size: 3.5rem; font-weight: 800; margin-bottom: 1rem; letter-spacing: -1px; }
        header p { font-size: 1.25rem; color: var(--text-dim); max-width: 600px; margin-bottom: 2rem; }

        .btn-primary {
            background: var(--primary);
            color: white;
            padding: 14px 28px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: 0.3s;
        }
        .btn-primary:hover { background: var(--primary-hover); transform: translateY(-2px); }

        /* --- Features Grid --- */
        .container { max-width: 1100px; margin: 0 auto; padding: 60px 20px; }
        
        .section-title { text-align: center; margin-bottom: 50px; font-size: 2rem; }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .feature-card {
            background: var(--card-bg);
            padding: 30px;
            border-radius: 16px;
            border: 1px solid rgba(255,255,255,0.1);
            transition: 0.3s;
        }
        .feature-card:hover { border-color: var(--primary); transform: translateY(-5px); }
        .feature-card h3 { margin-bottom: 10px; color: var(--primary); }

        /* --- Pricing Table --- */
        .pricing-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 30px;
            background: var(--card-bg);
            border-radius: 12px;
            overflow: hidden;
        }
        .pricing-table th, .pricing-table td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid rgba(255,255,255,0.05);
        }
        .pricing-table th { background: rgba(255,255,255,0.05); color: var(--primary); }

        /* --- Form Styling --- */
        .order-form {
            background: var(--card-bg);
            padding: 40px;
            border-radius: 20px;
            max-width: 700px;
            margin: 0 auto;
        }
        .form-group { margin-bottom: 20px; }
        label { display: block; margin-bottom: 8px; font-weight: 500; }
        input, select, textarea {
            width: 100%;
            padding: 12px;
            background: #0f172a;
            border: 1px solid #334155;
            color: white;
            border-radius: 6px;
        }
        input:focus { border-color: var(--primary); outline: none; }

        .cashapp-box {
            background: #00d63222;
            border: 1px dashed #00d632;
            padding: 20px;
            text-align: center;
            border-radius: 12px;
            margin-top: 40px;
        }

        footer { text-align: center; padding: 40px; color: var(--text-dim); font-size: 0.9rem; }
    </style>
</head>
<body>

    <header>
        <h1>THughes 3D</h1>
        <p>Custom 3D Prints On Demand. Fast, reliable, and professional-grade manufacturing for your wildest ideas.</p>
        <a href="#order" class="btn-primary">Start Your Project</a>
    </header>

    <div class="container">
        <h2 class="section-title">What We Offer</h2>
        <div class="features">
            <div class="feature-card">
                <h3>📦 Custom Prints</h3>
                <p>Upload your STL file. We print any safe and legal design with precision.</p>
            </div>
            <div class="feature-card">
                <h3>⚡ Fast Turnaround</h3>
                <p>Most prints completed in 1-5 business days depending on complexity.</p>
            </div>
            <div class="feature-card">
                <h3>🌍 Global Shipping</h3>
                <p>International shipping available. Costs calculated by weight and location.</p>
            </div>
            <div class="feature-card">
                <h3>✅ Quality Pro</h3>
                <p>Using professional-grade machines with strict quality control.</p>
            </div>
        </div>
    </div>

    <div class="container">
        <h2 class="section-title">Pricing Guide</h2>
        <table class="pricing-table">
            <thead>
                <tr>
                    <th>Size/Type</th>
                    <th>Price Range</th>
                    <th>Time</th>
                </tr>
            </thead>
            <tbody>
                <tr><td>Small (under 50g)</td><td>$15 - $40</td><td>1-2 Days</td></tr>
                <tr><td>Medium (50-200g)</td><td>$40 - $100</td><td>2-3 Days</td></tr>
                <tr><td>Large (200g+)</td><td>$100 - $250</td><td>3-5 Days</td></tr>
                <tr><td>Resin (High Detail)</td><td>$30 - $150</td><td>2-4 Days</td></tr>
            </tbody>
        </table>
    </div>

    <div class="container" id="order">
        <h2 class="section-title">Place Your Order</h2>
        <form class="order-form">
            <div class="form-group">
                <label>Your Name *</label>
                <input type="text" placeholder="John Doe" required>
            </div>
            <div class="form-group">
                <label>Email Address *</label>
                <input type="email" placeholder="john@example.com" required>
            </div>
            <div class="form-group">
                <label>Print Description *</label>
                <textarea rows="4" placeholder="Dimensions, material preference, and what you're building..."></textarea>
            </div>
            <div class="form-group">
                <label>Preferred Material</label>
                <select>
                    <option>PLA (Biodegradable)</option>
                    <option>PETG (Durable)</option>
                    <option>Resin (High Detail)</option>
                </select>
            </div>
            <div class="form-group">
                <label>Upload STL File (Optional)</label>
                <input type="file">
            </div>
            <button type="submit" class="btn-primary" style="width: 100%; border: none; cursor: pointer;">Send Order Request</button>
        </form>

        <div class="cashapp-box">
            <p><strong>Quick Questions?</strong></p>
            <p>Contact us via CashApp for fastest response: <span style="color: #00d632;">$TMHughes2025</span></p>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 THughes 3D Printing. All Rights Reserved.</p>
    </footer>

</body>
</html>
