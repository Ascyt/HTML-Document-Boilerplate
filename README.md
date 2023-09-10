<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Documentation</title>
</head>

<body>
  <div id="wrapper">
    <nav id="sidebar">
      <ul>
        <li>
          <a href="#">Title</a>
        </li>
        <li>
          <a href="#explanation">Explanation</a>
        </li>
        <li>
          <a href="#sections">Sections</a>
        </li>
        <li>
          <a href="#components">Components</a>
        </li>
      </ul>
    </nav>

    <div id="content">
      <div id="header">
        <section>
          <h1>Documentation</h1>
          <p>Ascyt</p>
          <p>10.09.2023</p>
        </section>
      </div>

      <section id="explanation">
        <h1>Explanation</h1>
        <p>This is a lightweight HTML boilerplate equipped with CSS.</p>
        <p>The CSS is included in this file so that you can send the HTML to anyone and have them open it up in their web browser without any issues.</p>
      </section>
      <section id="sections">
        <h1>Sections</h1>
        <p>Essentially, you just create sections for everything and add those sections to the sidebar.</p>

        <h4>An example of creating a new section:</h4>

        <p>First we put the section below the <code>&lt;div id="header"&gt; ... &lt;/div&gt;</code> block:</p>
        <pre>
&lt;section id="example"&gt;
  &lt;h1&gt;Example&lt;/h1&gt;
  &lt;p&gt;This is an example.&lt;/p&gt;
&lt;/section&gt;</pre>

          <p>Then we need to add the section to sidebar (found near the top), in the <code>&ltul&gt;</code> block:</p>
          <pre>
&lt;li&gt;
  &lt;a href="#example"&gt;Example&lt;/a&gt;
&lt;/li&gt;</pre>
        <p>Make sure the id of the section matches with the href of the link. </p>
      </section>

      <section id="components">
        <h1>Components</h1>
        <p>In the following you will see examples of HTML components you can use. Just use them like normal HTML components. For more information you can view this page's source (CTRL + U).</p>

        <div class="card" style="background-color: black;">
          <h1>&lt;h1&gt;</h1>
          <h2>&lt;h2&gt;</h2>
          <h3>&lt;h3&gt;</h3>
          <h4>&lt;h4&gt;</h4>
          <p>&lt;p&gt;</p>
          <p class="light">&lt;p class="light"&gt;</p>
          <p class="dark">&lt;p class="dark"&gt;</p>
          <a href="https://ascyt.com/">&lt;a href="https://ascyt.com/"&gt;</a>
          <p><code>&lt;code&gt;</code></p>
          <pre>&lt;pre&gt;</pre>
          <ul>
            <li>
              unordered list
            </li>
            <li>
              unordered list
              <ul>
                <li>
                  nested
                </li>
              </ul>
            </li>
          </ul>
          <ol>
            <li>
              ordered list
            </li>
            <li>
              ordered list
              <ol>
                <li>
                  nested
                </li>
              </ol>
            </li>
          </ol>
          <table>
            <tr>
              <th>
                table
              </th>
              <th>
                row
              </th>
              <th>
                header
              </th>
            </tr>
            <tr>
              <td>
                table
              </td>
              <td>
                row
              </td>
              <td>
                data
              </td>
            </tr>
            <tr>
              <td>
                table
              </td>
              <td>
                row
              </td>
              <td>
                data
              </td>
            </tr>
            <tr>
              <td>
                table
              </td>
              <td>
                row
              </td>
              <td>
                data
              </td>
            </tr>
            <tr>
              <td>
                table
              </td>
              <td>
                row
              </td>
              <td>
                data
              </td>
            </tr>
          </table>
          <div class="card">
            &lt;div class="card"&gt;
          </div>
        </div>
        
      </section>
      
      <a href="#" id="back-to-top">Back to top</a>
    </div>
  </div>
</body>

<style>
  html {
    scroll-behavior: smooth;
  }

  body {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: large;
    margin: 10px;
    text-align: left;
    background-color: #000000;
    color: #c0c0c0;
  }

  section {
    border-top-style: solid;
    border-top-width: 3px;
    border-color: #101010;

    padding-top: 10px;
    margin-bottom: 10px;
  }

  .light {
    color: #ffffff;
  }

  .dark {
    color: #808080;
  }

  .card {
    border-color: #808080;
    border-radius: 5px;
    border-width: 2px;
    border-style: solid;

    background-color: #101010;

    padding: 10px;
    margin-top: 10px;
    margin-bottom: 10px;
  }

  .card.dashed {
    border-style: dashed;
  }

  a {
    color: #40a6ff;
    transition: ease-out 0.3s;
  }

  a:hover {
    color: #2f7cbf;
    transition: ease-in-out 0.2s;
  }

  li {
    margin-left: -10px;
  }

  li>ul,
  ol>li {
    margin-left: -15px;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 10px;
    margin-bottom: 10px;
  }

  th {
    background-color: #202020;
    color: #ffffff;
  }

  th,
  td {
    padding: 8px;
    border: 1px solid #404040;
    border-style: solid;
    text-align: center;
  }

  tr:nth-child(odd) {
    background-color: #101010;
  }

  .invis>td {
    border-style: none;
  }

  
  pre, code {
    white-space: pre-wrap;
    overflow-x: auto;

    color: #c0c0c0;
    background-color: #101010;

    border-color: #808080;
    border-width: 1px;
    border-style: solid;
    border-right-style: solid;

    padding: 10px;

    border-radius: 5px;
  }

  code {
    padding: 2px;
    padding-left: 3px;
    padding-right: 3px;
  }

  #content {
    flex: 1;
    padding: 10px;
    padding-left: 5px;
  }

  #content h1 {
    color: #ffffff;
    text-align: center;
    margin-top: 0;
    margin-bottom: 10px;
  }
  #content h2 {
    color: #ffffff;
    text-decoration: underline;
    font-size: larger;
  }
  #content h3 {
    color: #ffffff;
    text-decoration: underline;
    font-size: large;
  }
  #content h4 {
    color: #ffffff;
    text-decoration: underline;
    font-size: large;
    font-weight: normal;
  }

  #header {
    text-align: center;
  }

  #header p,
  #header h1 {
    margin-bottom: -15px;
  }

  #header p {
    font-size: larger;
  }

  #header h1 {
    font-size: xx-large;
  }

  #header section {
    margin-bottom: 30px;
  }

  #wrapper {
    display: flex;
  }

  #sidebar {
    width: 15%;
    color: #fff;
  }

  #sidebar ul {
    list-style-type: none;
    padding: 0;

    position: fixed;
    width: 15%;

    margin-top: -10px;
    margin-left: -10px;

    max-height: 100vh;
    overflow-y: auto;
  }

  #sidebar ul li a {
    color: #fff;
    text-decoration: none;
    display: flex;
    padding-bottom: 10px;
    padding-top: 10px;
    padding-left: 10px;

    justify-content: center;
  }

  #sidebar ul li:nth-child(even) {
    background-color: #101010;

    transition: ease-out 0.15s;
  }

  #sidebar ul li:nth-child(even):hover {
    background-color: #303030;

    transition: ease-in-out 0.1s;
  }

  #sidebar ul li:nth-child(odd) {
    background-color: #202020;

    transition: ease-out 0.15s;
  }

  #sidebar ul li:nth-child(odd):hover {
    background-color: #303030;

    transition: ease-in-out 0.1s;
  }

  #back-to-top {
    border-color: #808080;
    border-radius: 5px;
    border-width: 2px;
    border-style: solid;

    margin-top: 10px;

    display: flex;
    justify-content: center;

    color: #c0c0c0;
    text-decoration: none;

    transition: ease-out 0.3s;
  }

  #back-to-top:hover {
    background-color: #202020;
    transition: ease-in-out 0.2s;
  }
</style>

</html>