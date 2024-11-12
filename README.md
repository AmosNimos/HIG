<body>
    <h1>HIG - Highlight In General</h1>
    <p><strong>Author:</strong> Amosnimos<br>
    <strong>License:</strong> GNU Affero General Public License</p>
    <p><strong>Description:</strong> HIG (Highlight In General): A simple bash utility to highlight specified words in piped or file input with customizable colors, preserving the original text.</p>

  <p><code>hig</code> is a utility developed by Amosnimos for highlighting specific words or phrases in text files or command output. It’s designed to bring easy, flexible highlighting to your command line experience, setting it apart from typical utilities like <code>grep</code>.</p>

  <h2>Features</h2>
    <ul>
        <li>Highlights specific keywords in piped or file input.</li>
        <li>Customize highlight color for text background or foreground.</li>
        <li>Supports both color inversion and foreground highlight modes.</li>
        <li>Accepts input directly from a file or from a pipe.</li>
        <li>Clean and easy to read – provides essential highlighting without altering text content.</li>
    </ul>

  <h2>Installation</h2>
    <p>Download the latest version of <code>hig</code> from GitHub:</p>
    <p><a href="https://github.com/Amosnimos/hig" target="_blank">https://github.com/Amosnimos/hig</a></p>

  <h2>Usage</h2>
    <p>Use <code>hig</code> to highlight specific words or phrases in text from either a file or pipe input. Below are some examples:</p>

  <h3>Examples</h3>
    <p>Basic usage with pipe input:</p>
    <pre><code>
echo "hello world" | hig -s world
    </code></pre>
    <p>Specifying a background highlight color:</p>
    <pre><code>
echo "hello world" | hig -s world -c red
    </code></pre>

<p>Using a file as input:</p>
<pre><code>
hig -s "search_term" -f /path/to/file.txt -c green
</code></pre>

<p>Inverting colors to highlight text instead of the background:</p>
<pre><code>
echo "hello world" | hig -s world -i -c yellow</code></pre>
</code></pre>

  <h3>Options</h3>
    <ul>
        <li><code>-s</code>, <code>--search &lt;term&gt;</code>: The term or phrase to highlight.</li>
        <li><code>-f</code>, <code>--file &lt;filename&gt;</code>: Use a file as input instead of pipe data.</li>
        <li><code>-c</code>, <code>--color &lt;color&gt;</code>: Background color for highlighting (default: yellow).</li>
        <li><code>-i</code>, <code>--invert</code>: Inverts color to highlight text instead of background.</li>
        <li><code>-h</code>, <code>--help</code>: Display help information.</li>
    </ul>

  <h2>Why hig?</h2>
    <p><code>hig</code> was built for cases where you need to <strong>visually highlight</strong> a word or phrase without filtering lines like <code>grep</code>. Here’s how it’s different:</p>
    <ul>
        <li><strong>No filtering:</strong> <code>hig</code> keeps all content and simply adds color to your keyword.</li>
        <li><strong>Color flexibility:</strong> Customize highlight color for quick visual scanning.</li>
        <li><strong>Readability:</strong> Useful for highlighting terms in logs or output without removing lines.</li>
    </ul>

  <h2>License</h2>
    <p class="license">
        <code>hig</code> is licensed under the GNU Affero General Public License (AGPL), ensuring users' freedom to run, share, and modify the software. For full license details, see the <a href="https://www.gnu.org/licenses/agpl-3.0.en.html" target="_blank">GNU AGPL-3.0 License</a>.
    </p>

  <footer>
      <p>Developed by Amosnimos, 2024</p>
  </footer>
</body>
</html>

