<h2>Prerequisite and Execution</h2>
<h3>Prerequisite</h3>
<ol>
  <li>Download and install the latest version of <a href="https://www.python.org/downloads/" target="_blank">Python</a>.</li>
  <li>Make sure you have the <a href="https://www.google.com/chrome/" target="_blank">Google Chrome browser</a> installed.</li>
  <li>Install Required Tools:</li>
  <ul>
    <li>Open Command Prompt (type <code>cmd</code> in Windows search).</li>
    <li>Run the following commands to install the necessary tools:
      <ul>
        <li><code>pip install selenium</code></li>
        <li><code>pip install webdriver-manager</code></li>
      </ul>
      <p>These are like installing extra tools that help Python control the web browser.</p>
    </li>
  </ul>
</ol>

<h3>Execution</h3>
<ol>
  <li>Open Python and create a new file.</li>
  <li>Copy the script (attached below) and paste it into the file.</li>
  <li>Save the file as <code>Fitpeo_Assignment.py</code>.</li>
  <li>To run the script:
    <ol>
      <li>Open Command Prompt.</li>
      <li>Navigate to the file location using the command: <code>cd file_path</code>.</li>
      <li>Run the script using: <code>python filename.py</code> (e.g., <code>python Fitpeo_Assignment.py</code>).</li>
    </ol>
  </li>
  <li>Output:
    <ul>
      <li>Chrome will open automatically and perform all the functions mentioned in the script.</li>
      <li>Messages will appear in the Command Prompt showing what the script is doing.</li>
    </ul>
  </li>
</ol>


<p>********************************************</p>

<h2>Steps Covered in the Script</h2>

<h3>First Setup</h3>
<ul>
  <li>Opens Google Chrome browser</li>
  <li>Sets up some special browser settings to make automation smoother</li>
  <li>Makes sure we have the right version of ChromeDriver that matches your Chrome browser</li>
</ul>

<h3>Navigation</h3>
<ul>
  <li>Goes directly to the <a href="https://www.fitpeo.com/revenue-calculator" target="_blank">FitPeo Revenue Calculator</a> page</li>
  <li>Waits for the page to load completely</li>
  <li>Verifies we're on the right page</li>
</ul>

<h3>Finding and Setting Up the Slider</h3>
<ul>
  <li>Scrolls down the page until it finds the patient number slider</li>
  <li>Makes sure the slider is visible on screen</li>
  <li>Gets ready to interact with both the slider and its associated text input field</li>
</ul>

<h3>Adjusting Patient Numbers</h3>
<ul>
  <li>First sets the value to <strong>820 patients</strong> by:
    <ul>
      <li>Finding the number input field</li>
      <li>Clearing any existing value</li>
      <li>Typing in "820"</li>
      <li>Pressing Enter to confirm</li>
    </ul>
  </li>
  <li>Then changes it to <strong>560 patients</strong> using the same method</li>
  <li>Waits between adjustments to let the page update</li>
</ul>

<h3>Selecting CPT Codes</h3>
<ul>
  <li>Looks for four specific CPT code checkboxes:
    <ul>
      <li><strong>CPT-99091</strong></li>
      <li><strong>CPT-99453</strong></li>
      <li><strong>CPT-99454</strong></li>
      <li><strong>CPT-99474</strong></li>
    </ul>
  </li>
  <li>For each code:
    <ul>
      <li>Finds the checkbox</li>
      <li>Clicks it to select</li>
      <li>Waits a moment to ensure the selection is registered</li>
    </ul>
  </li>
</ul>

<h3>Verifying the Results</h3>
<ul>
  <li>Looks for the <strong>"Total Recurring Reimbursement"</strong> amount</li>
  <li>Gets the displayed value</li>
  <li>Removes the "$" sign and any commas</li>
  <li>Compares it to the expected value of <strong>$110,700</strong></li>
  <li>Reports whether the amounts match</li>
</ul>

<h3>Error Handling Throughout</h3>
<ul>
  <li>At each step, the script:
    <ul>
      <li>Tries multiple ways to find elements if the first attempt fails</li>
      <li>Waits patiently for elements to appear</li>
      <li>Reports detailed information about what it's doing</li>
      <li>Catches and reports any errors that occur</li>
    </ul>
  </li>
</ul>

<h3>Cleanup</h3>
<ul>
  <li>After all steps are complete (or if something goes wrong):</li>
  <ul>
    <li>Properly closes the browser</li>
    <li>Reports the final status of the test</li>
  </ul>
</ul>






