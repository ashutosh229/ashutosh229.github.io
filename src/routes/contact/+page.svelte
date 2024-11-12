<script>
  import Fa from "svelte-fa/src/fa.svelte";
  import {
    faPhoneAlt,
    faEnvelope,
    faMapMarkedAlt,
  } from "@fortawesome/free-solid-svg-icons";

  import SectionHeader from "$lib/components/SectionHeader.svelte";
  let heading = "Contact Us";

  let isClicked = false;
  function handleClick() {
    isClicked = !isClicked;
    console.log(isClicked);
  }
  let isClicked2 = false;
  function handleClick2() {
    isClicked2 = !isClicked2;
    console.log(isClicked2);
  }
  let isClicked3 = false;
  function handleClick3() {
    isClicked3 = !isClicked3;
    console.log(isClicked3);
  }
  let isClicked4 = false;
  function handleClick4() {
    isClicked4 = !isClicked4;
    console.log(isClicked4);
  }
  let isClicked5 = false;
  function handleClick5() {
    isClicked5 = !isClicked5;
    console.log(isClicked5);
  }
  let isClicked6 = false;
  function handleClick6() {
    isClicked6 = !isClicked6;
    console.log(isClicked6);
  }
</script>

<svelte:head>
  <title>Contact | Meraz'24</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cormorant+Upright:wght@300;400;500;600;700&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap"
    rel="stylesheet"
  />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cormorant+Upright:wght@300;400;500;600;700&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<div class="back">
  <div class="aboutmeraz">
    <SectionHeader bind:name={heading} />
  </div>

  <div
    class="parent"
    style="background:rgb(66, 66, 66, 25%);	border-radius: 12px;"
  >
    <div class="top">
      <iframe
        title="IIT Bhilai Map"
        id="map-iframe"
        src="https://maps.google.com/maps?width=700&amp;height=440&amp;hl=en&amp;q=IIT%20Bhilai+(Meraz)&amp;ie=UTF8&amp;t=&amp;z=12&amp;iwloc=B&amp;output=embed"
        frameborder="0"
        scrolling="no"
        marginheight="0"
        marginwidth="0"
      />
    </div>
    <div class="bottom">
      <div class="team" id="info">
        <h2>
          <Fa icon={faPhoneAlt} />
          <span>Phone</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Himanshu Rana (CoSA President) - 8770571371</p>
            <p>Harsh Meena (CoSA Events Head) - 7611088018</p>
            <p>Piyush Chandrakar (CoSA Treasurer) - 9179932361</p>
            <p>Ojus Goel (Scitech Convenor) - 8708943859</p>
            <p>Smit Maurya (Culturals Convenor) - 7985370417</p>
            <p>Aditya Prakash (Informals Convenor) - 8335025833</p>
            <p>Uttkrist chouksey (Sports Convenor) - 6268533675</p>
          </div>
        </div>
      </div>

      <div class="team" id="info">
        <h2>
          <Fa icon={faEnvelope} />
          <span>E-mail</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>
              <a href="mailto:President_CoSA@iitbhilai.ac.in"
                >president_CoSA@iitbhilai.ac.in
              </a>
            </p>
            <p>
              <a href="mailto:eventshead_cosa@iitbhilai.ac.in"
                >eventshead_cosa@iitbhilai.ac.in
              </a>
            </p>
          </div>
        </div>
      </div>

      <div class="team" id="info">
        <h2>
          <Fa icon={faPhoneAlt} />
          <span>Address</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>
              Indian Institute of Technology Bhilai <br />
              Kutelabhata, Durg Chhattisgarh <br />
              India - 491002
            </p>
          </div>
        </div>
      </div>
      <div class="team" id="info" on:click={handleClick}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Registration and Help Desk</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Ayush Kumar - 9279020055</p>
            <p>Himanshu Soni - 9119219983</p>
            <p>(Only Whatsapp Calls and Messages are allowed)</p>
          </div>
        </div>
      </div>

      <div class="team" id="info" on:click={handleClick2}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Transportation</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Haisam - 7307627168</p>
            <p>Amritansh - 8709730535</p>
          </div>
        </div>
      </div>

      <div class="team" id="info" on:click={handleClick3}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Hospitality</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Nayan - 8223823011</p>
            <p>Himanshi - 8307125572</p>
          </div>
        </div>
      </div>

      <div class="team" id="info" on:click={handleClick4}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Security</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Ankit - 9350495775</p>
            <p>Sachin - 6205042648</p>
          </div>
        </div>
      </div>

      <div class="team" id="info" on:click={handleClick5}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Ground Force</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Tanishq Gupta - 8955947415</p>
            <p>Nitin Dhankar - 9256357600</p>
            <p>Sanjay Nimroth - 8949424140</p>
          </div>
        </div>
      </div>

      <div class="team" id="info" on:click={handleClick6}>
        <h2>
          <Fa icon={faEnvelope} />
          <span>Sponsorship</span>
        </h2>
        <div class="nonhiddenInfo">
          <div id="poc">
            <p>Akash Patel - 9460568832</p>
            <p>Nayan Jain - 8223823011</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<style lang="scss">
  * {
    color: white;
  }
  #info {
    padding: 20px;
  }
  .hiddenInfo {
    display: none;
    padding: 10px;
    margin-top: 10px;
  }
  .nonhiddenInfo {
    padding: 10px;
    margin-top: 10px;
  }
  .team {
    width: 30%;
    padding: 15px;
    color: black;
    text-align: center;
    min-width: 350px;
  }
  .bottom {
    margin-top: 10px;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    margin-bottom: 50px;
    flex-wrap: wrap;
  }

  .back {
    background-color: rgba(2, 11, 26, 0.92);
    height: auto;
    padding: 10px;
    background-repeat: no-repeat;
    background-size: cover;
  }

  .parent {
    scroll-snap-align: start;
    scroll-margin-top: 75px;
    background-color: rgba(34, 127, 173, 0.1);

    object-fit: cover;
    border-radius: 12px;
    margin: 10px;
    border-width: 3px;
    border-style: solid;
    border: 1 round solid rgb(177, 177, 177);
  }

  .top {
    display: flex;
  }

  span {
    font-family: "Josefin Sans", sans-serif;
  }

  h2 {
    font-weight: normal;
    font-family: "Cormorant Upright", serif;
    span {
      color: transparent;
      background: rgb(255, 255, 255);
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
  }

  p,
  a {
    font-family: "Libre Baskerville", serif;
    font-size: 16px;
  }

  iframe {
    width: 100%;
    margin: 40px;
    height: 460px;
  }
  @media (min-width: 800px) {
    .parent {
      margin: 75px;
      padding: 10px;
    }
  }
  @media (max-width: 800px) {
    .back {
      height: auto;
    }
    .parent {
      flex-direction: column;
    }
    iframe {
      margin: 20px;
      width: 90%;
      height: 200px;
    }
    .team {
      min-width: 100%;
    }
  }
</style>
