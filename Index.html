<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Confessions</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
      background: linear-gradient(135deg, #141e30, #243b55);
      color: white;
    }

    .container {
      width: 100%;
      max-width: 520px;
    }

    .card {
      background: rgba(255,255,255,.09);
      backdrop-filter: blur(18px);
      border: 1px solid rgba(255,255,255,.15);
      border-radius: 24px;
      padding: 30px;
      box-shadow: 0 20px 50px rgba(0,0,0,.35);
    }

    .icon {
      text-align: center;
      font-size: 48px;
      margin-bottom: 8px;
    }

    h1 {
      text-align: center;
      font-size: 29px;
      margin-bottom: 8px;
    }

    .subtitle {
      text-align: center;
      color: #cbd5e1;
      font-size: 14px;
      line-height: 1.5;
      margin-bottom: 25px;
    }

    label {
      display: block;
      font-size: 14px;
      font-weight: bold;
      margin-bottom: 8px;
    }

    textarea {
      width: 100%;
      height: 190px;
      resize: vertical;
      min-height: 120px;
      max-height: 350px;
      padding: 15px;
      border: none;
      outline: none;
      border-radius: 15px;
      background: white;
      color: #111827;
      font-size: 15px;
      line-height: 1.5;
    }

    textarea::placeholder {
      color: #6b7280;
    }

    .counter {
      text-align: right;
      color: #cbd5e1;
      font-size: 12px;
      margin-top: 6px;
      margin-bottom: 18px;
    }

    button {
      width: 100%;
      padding: 15px;
      border: none;
      border-radius: 15px;
      background: white;
      color: #243b55;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      transition: .2s;
    }

    button:hover {
      transform: translateY(-2px);
    }

    button:active {
      transform: scale(.98);
    }

    button:disabled {
      opacity: .6;
      cursor: not-allowed;
      transform: none;
    }

    .notice {
      text-align: center;
      margin-top: 18px;
      color: #aebaca;
      font-size: 11px;
      line-height: 1.5;
    }

    .success {
      display: none;
      text-align: center;
    }

    .success-icon {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .success h2 {
      margin-bottom: 10px;
    }

    .success p {
      color: #cbd5e1;
      font-size: 14px;
      line-height: 1.5;
      margin-bottom: 20px;
    }

    .again {
      background: transparent;
      border: 1px solid rgba(255,255,255,.3);
      color: white;
    }

    .error {
      display: none;
      margin-top: 15px;
      padding: 12px;
      border-radius: 10px;
      background: rgba(255, 80, 80, .15);
      color: #fecaca;
      text-align: center;
      font-size: 13px;
    }

    @media (max-width: 480px) {
      .card {
        padding: 23px;
      }

      h1 {
        font-size: 25px;
      }
    }
  </style>
</head>

<body>

  <main class="container">

    <section class="card">

      <div id="formSection">

        <div class="icon">💭</div>

        <h1>Secret Confessions</h1>

        <p class="subtitle">
          Have something you want to say?<br>
          Share it without putting your name.
        </p>

        <!-- REAL SUBMISSION FORM -->
        <form
          id="confessionForm"
          action="YOUR_FORMSPREE_ENDPOINT"
          method="POST"
        >

          <label for="confession">
            Your confession
          </label>

          <textarea
            id="confession"
            name="confession"
            maxlength="1000"
            placeholder="Write your confession here..."
            required
          ></textarea>

          <div class="counter">
            <span id="count">0</span>/1000
          </div>

          <!-- Helps identify the form in your dashboard -->
          <input
            type="hidden"
            name="_subject"
            value="New Anonymous Confession"
          >

          <button id="submitButton" type="submit">
            Send Confession 💌
          </button>

          <div class="error" id="errorMessage">
            Something went wrong. Please try again.
          </div>

        </form>

        <p class="notice">
          🔒 Don't include passwords, addresses, phone numbers,
          or other private information.
        </p>

      </div>


      <div class="success" id="successSection">

        <div class="success-icon">💌</div>

        <h2>Confession Sent!</h2>

        <p>
          Your confession was successfully submitted.
          Thank you for sharing.
        </p>

        <button
          class="again"
          onclick="showForm()"
          type="button"
        >
          Send Another
        </button>

      </div>

    </section>

  </main>


  <script>

    const form =
      document.getElementById("confessionForm");

    const confession =
      document.getElementById("confession");

    const counter =
      document.getElementById("count");

    const button =
      document.getElementById("submitButton");

    const error =
      document.getElementById("errorMessage");

    const formSection =
      document.getElementById("formSection");

    const successSection =
      document.getElementById("successSection");


    // Character counter
    confession.addEventListener("input", () => {
      counter.textContent = confession.value.length;
    });


    // Submit confession
    form.addEventListener("submit", async (event) => {

      event.preventDefault();

      const text = confession.value.trim();

      if (!text) {
        return;
      }

      button.disabled = true;
      button.textContent = "Sending... 💌";
      error.style.display = "none";

      try {

        const response = await fetch(
          form.action,
          {
            method: "POST",
            body: new FormData(form),
            headers: {
              "Accept": "application/json"
            }
          }
        );

        if (response.ok) {

          confession.value = "";
          counter.textContent = "0";

          formSection.style.display = "none";
          successSection.style.display = "block";

        } else {

          throw new Error("Submission failed");

        }

      } catch (err) {

        error.style.display = "block";

      } finally {

        button.disabled = false;
        button.textContent = "Send Confession 💌";

      }

    });


    function showForm() {

      successSection.style.display = "none";
      formSection.style.display = "block";

    }

  </script>

</body>
</html>
