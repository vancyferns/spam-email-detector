<h1>📧 Spam Email Detector</h1>

<p>A web-based spam detection system built with Flask and Machine Learning.</p>

<h2>🚀 Features</h2>
<ul>
  <li>Detects whether an email is spam or not</li>
  <li>Flask-powered web interface</li>
  <li>Pre-trained model using scikit-learn</li>
  <li>Simple and clean UI</li>
</ul>

<h2>🧠 Tech Stack</h2>
<ul>
  <li><strong>Backend:</strong> Python, Flask, scikit-learn</li>
  <li><strong>Frontend:</strong> HTML, CSS (via templates)</li>
  <li><strong>Deployment:</strong> Gunicorn on Render</li>
  <li><strong>Development Environment:</strong> GitHub Codespaces</li>
</ul>

<h2>📂 Project Structure</h2>
<pre>
├── app.py                # Flask app entry point
├── utils.py              # Helper functions for prediction
├── models/
│   ├── cv.pkl            # CountVectorizer object
│   └── clf.pkl           # Trained classification model
├── templates/
│   └── index.html        # Main frontend HTML page
├── requirements.txt      # Python dependencies
├── runtime.txt           # Python runtime version
├── README.md             # Project documentation
</pre>

<h2>🔍 How It Works</h2>
<ol>
  <li>User enters the email content into the input form on the web page.</li>
  <li>The input is sent to the Flask backend via POST request.</li>
  <li>The text is vectorized using a pre-trained <code>CountVectorizer</code> (cv.pkl).</li>
  <li>The vector is then passed to the trained classifier model (clf.pkl).</li>
  <li>The model predicts whether the email is spam or not.</li>
  <li>The prediction result is displayed back to the user on the same page.</li>
</ol>

<h2>⚙️ How to Run Locally</h2>
<ol>
  <li>Clone the repository</li>
  <li>Create and activate a virtual environment</li>
  <li>Install dependencies:
    <pre><code>pip install -r requirements.txt</code></pre>
  </li>
  <li>Run the Flask app:
    <pre><code>python app.py</code></pre>
  </li>
  <li>Open <code>http://localhost:5000</code> in your browser</li>
</ol>

<h2>🌐 Deployment</h2>
<p>This project is deployed live using <strong>Render</strong> cloud platform.</p>
<p>Development and testing were done in <strong>GitHub Codespaces</strong>, providing a consistent cloud-based dev environment.</p>

<h2>✅ Sample Inputs</h2>
<h3>Spam Email:</h3>
<pre>
Congratulations! You’ve won a $1,000 gift card.
Click here to claim your prize now!
</pre>

<h3>Non-Spam Email:</h3>
<pre>
Hi Team,

This is a reminder about tomorrow's 10 AM project sync.
Please be prepared with your sprint updates.

Best,
John
</pre>

<h2>📜 License</h2>
<p>MIT License</p>
