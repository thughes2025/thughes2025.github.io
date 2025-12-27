# thughes2025.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3D Printing Services - Custom Prints On Demand</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem 0;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.95;
        }

        nav {
            background-color: #333;
            padding: 1rem 0;
            text-align: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #667eea;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        section {
            margin: 3rem 0;
        }

        section h2 {
            color: #667eea;
            margin-bottom: 1.5rem;
            font-size: 2rem;
            border-bottom: 3px solid #667eea;
            padding-bottom: 0.5rem;
            display: inline-block;
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .feature-card {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 4px solid #667eea;
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 12px rgba(102, 126, 234, 0.2);
        }

        .feature-card h3 {
            color: #667eea;
            margin-bottom: 0.5rem;
        }

        .specs {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            margin: 1.5rem 0;
        }

        .specs h3 {
            color: #667eea;
            margin-bottom: 1rem;
        }

        .spec-item {
            display: flex;
            justify-content: space-between;
            padding: 0.75rem 0;
            border-bottom: 1px solid #ddd;
        }

        .spec-item:last-child {
            border-bottom: none;
        }

        .spec-label {
            font-weight: 600;
            color: #333;
        }

        .spec-value {
            color: #666;
        }

        .pricing-table {
            width: 100%;
            border-collapse: collapse;
            margin: 1.5rem 0;
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        .pricing-table th {
            background-color: #667eea;
            color: white;
            padding: 1rem;
            text-align: left;
            font-weight: 600;
        }

        .pricing-table td {
            padding: 1rem;
            border-bottom: 1px solid #ddd;
        }

        .pricing-table tr:last-child td {
            border-bottom: none;
        }

        .pricing-table tr:hover {
            background-color: #f8f9fa;
        }

        .warning-box {
            background-color: #fff3cd;
            border-left: 4px solid #ffc107;
            padding: 1.5rem;
            border-radius: 4px;
            margin: 1.5rem 0;
        }

        .warning-box h4 {
            color: #856404;
            margin-bottom: 0.5rem;
        }

        .warning-box p {
            color: #856404;
        }

        .cta-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 2rem;
            border-radius: 8px;
            text-align: center;
            margin: 2rem 0;
        }

        .cta-section h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .btn {
            display: inline-block;
            background-color: #667eea;
            color: white;
            padding: 0.75rem 2rem;
            text-decoration: none;
            border-radius: 5px;
            font-weight: 600;
            transition: background-color 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            margin: 0.5rem;
        }

        .btn:hover {
            background-color: #764ba2;
        }

        .btn-secondary {
            background-color: white;
            color: #667eea;
        }

        .btn-secondary:hover {
            background-color: #f0f0f0;
        }

        .order-form {
            background: #f8f9fa;
            padding: 2rem;
            border-radius: 8px;
            max-width: 600px;
            margin: 2rem auto;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #333;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: inherit;
            font-size: 1rem;
        }

        .form-group textarea {
            resize: vertical;
            min-height: 100px;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }

        .checkbox-group {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .checkbox-group input {
            width: auto;
            margin: 0;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
        }

        .contact-info {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            margin: 1.5rem 0;
            text-align: center;
        }

        .contact-info p {
            margin: 0.5rem 0;
            font-size: 1.1rem;
        }

        .contact-link {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
        }

        .contact-link:hover {
            text-decoration: underline;
        }

        .deposit-highlight {
            background-color: #ffe5e5;
            border-left: 4px solid #dc3545;
            padding: 1rem;
            border-radius: 4px;
            margin: 1rem 0;
        }

        .deposit-highlight strong {
            color: #dc3545;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.8rem;
            }

            nav a {
                display: block;
                margin: 0.5rem 0;
            }

            .container {
                padding: 1rem;
            }

            .features {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>🖨️ 3D Printing Services</h1>
        <p>Custom 3D Prints On Demand - Fast, Reliable, Professional</p>
    </header>

    <nav>
        <a href="#services">Services</a>
        <a href="#specs">Specifications</a>
        <a href="#pricing">Pricing</a>
        <a href="#order">Place Order</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container">
        <!-- Services Section -->
        <section id="services">
            <h2>What We Offer</h2>
            <div class="features">
                <div class="feature-card">
                    <h3>📦 Custom Prints</h3>
                    <p>We print any safe and legal design. Upload your STL file or provide specifications, and we'll bring your ideas to life.</p>
                </div>
                <div class="feature-card">
                    <h3>⚡ Fast Turnaround</h3>
                    <p>Competitive pricing with quick production times. Most prints completed within 1-5 business days depending on complexity.</p>
                </div>
                <div class="feature-card">
                    <h3>🌍 Worldwide Shipping</h3>
                    <p>We ship internationally. Shipping costs calculated based on location and package weight.</p>
                </div>
                <div class="feature-card">
                    <h3>✅ Quality Guaranteed</h3>
                    <p>Professional-grade 3D printers with careful quality control. Your satisfaction is our priority.</p>
                </div>
            </div>
        </section>

        <!-- Specifications Section -->
        <section id="specs">
            <h2>Print Specifications</h2>
            
            <div class="specs">
                <h3>Standard Print Dimensions</h3>
                <div class="spec-item">
                    <span class="spec-label">Maximum Standard Size:</span>
                    <span class="spec-value">220mm × 220mm × 220mm</span>
                </div>
                <div class="spec-item">
                    <span class="spec-label">Minimum Feature Size:</span>
                    <span class="spec-value">0.4mm</span>
                </div>
                <div class="spec-item">
                    <span class="spec-label">Print Accuracy:</span>
                    <span class="spec-value">±0.3mm</span>
                </div>
            </div>

            <div class="deposit-highlight">
                <strong>⚠️ Important - Large Print Orders:</strong><br>
                Orders exceeding 220mm × 220mm × 220mm require:
                <ul style="margin-left: 1.5rem; margin-top: 0.5rem;">
                    <li>Prior approval from our team</li>
                    <li>$50 deposit (non-refundable, applied to final cost)</li>
                </ul>
                Contact us before placing large orders.
            </div>

            <div class="specs">
                <h3>Materials Available</h3>
                <div class="spec-item">
                    <span class="spec-label">PLA Filament:</span>
                    <span class="spec-value">Biodegradable, various colors</span>
                </div>
                <div class="spec-item">
                    <span class="spec-label">PETG Filament:</span>
                    <span class="spec-value">Durable, impact resistant</span>
                </div>
                <div class="spec-item">
                    <span class="spec-label">Resin Printing:</span>
                    <span class="spec-value">Available for high-detail prints</span>
                </div>
            </div>

            <div class="warning-box">
                <h4>What We Cannot Print</h4>
                <p>We cannot print items that are illegal, unsafe, or violate intellectual property rights. This includes weapons, counterfeit items, or anything designed to cause harm. All orders must be safe and legal.</p>
            </div>
        </section>

        <!-- Pricing Section -->
        <section id="pricing">
            <h2>Pricing</h2>
            <p>Pricing is calculated based on material volume, complexity, and print time. Here's an approximate guide:</p>
            
            <table class="pricing-table">
                <thead>
                    <tr>
                        <th>Print Size/Type</th>
                        <th>Estimated Price Range</th>
                        <th>Turnaround Time</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Small Print (under 50g)</td>
                        <td>$15 - $40</td>
                        <td>1-2 days</td>
                    </tr>
                    <tr>
                        <td>Medium Print (50-200g)</td>
                        <td>$40 - $100</td>
                        <td>2-3 days</td>
                    </tr>
                    <tr>
                        <td>Large Print (200g+, under 220³mm)</td>
                        <td>$100 - $250</td>
                        <td>3-5 days</td>
                    </tr>
                    <tr>
                        <td>Custom/Extra Large (approval required)</td>
                        <td>Custom quote + $50 deposit</td>
                        <td>5+ days</td>
                    </tr>
                    <tr>
                        <td>Resin Prints (high detail)</td>
                        <td>$30 - $150</td>
                        <td>2-4 days</td>
                    </tr>
                </tbody>
            </table>

            <p style="margin-top: 1rem; font-style: italic; color: #666;">Shipping costs calculated at checkout based on location and weight. Contact us for exact pricing on your specific project.</p>
        </section>

        <!-- Order Section -->
        <section id="order">
            <h2>Place Your Order</h2>
            <p style="margin-bottom: 1.5rem;">Ready to get your prints made? Fill out the form below or contact us directly.</p>
            
            <form class="order-form" onsubmit="handleOrderSubmit(event)">
                <div class="form-group">
                    <label for="name">Your Name *</label>
                    <input type="text" id="name" name="name" required>
                </div>

                <div class="form-group">
                    <label for="email">Email Address *</label>
                    <input type="email" id="email" name="email" required>
                </div>

                <div class="form-group">
                    <label for="phone">Phone Number</label>
                    <input type="tel" id="phone" name="phone">
                </div>

                <div class="form-group">
                    <label for="description">Print Description *</label>
                    <textarea id="description" name="description" placeholder="Describe what you want printed. Include dimensions, material preference, etc." required></textarea>
                </div>

                <div class="form-group">
                    <label for="dimensions">Approximate Dimensions (mm) *</label>
                    <input type="text" id="dimensions" name="dimensions" placeholder="e.g., 100x100x50" required>
                </div>

                <div class="form-group">
                    <label for="material">Preferred Material</label>
                    <select id="material" name="material">
                        <option value="">Select material...</option>
                        <option value="pla">PLA Filament</option>
                        <option value="petg">PETG Filament</option>
                        <option value="resin">Resin (High Detail)</option>
                        <option value="unsure">Not sure - recommend something</option>
                    </select>
                </div>

                <div class="form-group">
                    <label for="file">Upload STL File (optional)</label>
                    <input type="file" id="file" name="file" accept=".stl,.obj">
                </div>

                <div class="form-group">
                    <div class="checkbox-group">
                        <input type="checkbox" id="large" name="large">
                        <label for="large" style="margin: 0;">This print exceeds 220mm × 220mm × 220mm</label>
                    </div>
                </div>

                <div class="form-group">
                    <label for="notes">Additional Notes</label>
                    <textarea id="notes" name="notes" placeholder="Any special requirements or questions?"></textarea>
                </div>

                <button type="submit" class="btn" style="width: 100%; font-size: 1.1rem;">Send Order Request</button>
            </form>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2>Get In Touch</h2>
            <div class="contact-info">
                <p><strong>Quick Questions?</strong></p>
                <p>Contact us via CashApp for fastest response:</p>
                <p style="margin-top: 1rem; font-size: 1.3rem;">
                    <a href="https://cash.app/$TMHughes2025" class="contact-link">💰 $TMHughes2025</a>
                </p>
                <p style="margin-top: 1rem; color: #666;">Send payment requests or deposits directly through CashApp for fastest service.</p>
            </div>
        </section>

        <div class="cta-section">
            <h3>Ready to Get Started?</h3>
            <p>Submit your print request above and we'll get back to you with a quote and timeline!</p>
        </div>
    </div>

    <footer>
        <p>&copy; 2025 3D Printing Services. All prints must be safe and legal. We reserve the right to decline orders.</p>
        <p style="margin-top: 1rem; font-size: 0.9rem;">Large orders (220mm+) require prior approval and $50 deposit.</p>
    </footer>

    <script>
        function handleOrderSubmit(event) {
            event.preventDefault();
            
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const phone = document.getElementById('phone').value;
            const description = document.getElementById('description').value;
            const dimensions = document.getElementById('dimensions').value;
            const material = document.getElementById('material').value;
            const large = document.getElementById('large').checked;
            const notes = document.getElementById('notes').value;
            
            // Create email body
            let emailBody = `New Print Order Request:\n\n`;
            emailBody += `Name: ${name}\n`;
            emailBody += `Email: ${email}\n`;
            emailBody += `Phone: ${phone || 'Not provided'}\n\n`;
            emailBody += `Print Description:\n${description}\n\n`;
            emailBody += `Dimensions: ${dimensions}mm\n`;
            emailBody += `Preferred Material: ${material || 'Not specified'}\n`;
            emailBody += `Large Order (needs approval): ${large ? 'Yes - requires $50 deposit' : 'No'}\n`;
            emailBody += `Additional Notes:\n${notes || 'None'}\n`;
            
            // For now, show confirmation and instructions
            alert(`Thank you for your order request!\n\nPlease send the details below to confirm via CashApp or email:\n\n${emailBody}\n\nWe'll review your request and get back to you within 24 hours with a quote and timeline.`);
            
            // Reset form
            document.querySelector('.order-form').reset();
        }
    </script>
</body>
</html>
