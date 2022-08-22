<template>
  <div class="__HomeScreen">
    <div class="__toggle">
      <i @click="toggleUp" class="fa-solid fa-xmark"></i>
      <nav class="__Nav">
        <li><a href="#">Our vehicules</a></li>
        <li><a href="#">About transport society</a></li>
        <li><a href="#">The refrigeration specialist</a></li>
        <li><a href="#">Full service!</a></li>
        <li><a href="#">Our agencies</a></li>
        <div class="__Region">
          <img
            src="../assets/Templtaes-NP/south-africa.png"
            alt="south-africa.png"
          />
          <div class="__Safrica">
            <p>South Africa</p>
            <i class="fa-solid fa-angle-down"></i>
          </div>
        </div>
      </nav>
    </div>
    <header
      data-aos="fade-down"
      data-aos-easing="linear"
      data-aos-duration="1000"
      class="__Header"
    >
      <a href="#" class="__Logo">
        <img
          src="../assets/Templtaes-NP/logo.png"
          alt="Logo Transport Society"
          title="Logo Transport Society"
          width="80"
        />
        <div class="__LogoText">
          Transport <br />
          Society
        </div>
      </a>
      <!-- § -->
      <nav class="__Nav">
        <li><a href="#">Our vehicules</a></li>
        <li><a href="#">About transport society</a></li>
        <li><a href="#">The refrigeration specialist</a></li>
        <li><a href="#">Full service!</a></li>
        <li><a href="#">Our agencies</a></li>
        <div class="__Region">
          <img
            src="../assets/Templtaes-NP/south-africa.png"
            alt="south-africa.png"
          />
          <div class="__Safrica">
            <p>South Africa</p>
            <i class="fa-solid fa-angle-down"></i>
          </div>
        </div>
      </nav>
      <i @click="toggle" class="fa-solid fa-align-right"></i>
    </header>
    <!-- § -->
    <section
      data-aos="fade-left"
      data-aos-anchor="#example-anchor"
      data-aos-offset="500"
      data-aos-duration="500"
      class="__SauteOYeux"
      id="__SauteOYeux"
    >
      <div class="__PresentationContainer" id="__PresentationContainer">
        <div id="__soyt">
          <h1
            data-aos="fade-right"
            data-aos-offset="300"
            data-aos-easing="ease-in-sine"
            id="__h1r"
          >
            Refrigerated vehicle <br />
            rental
          </h1>
          <p
            class="__p1r"
            data-aos="fade-left"
            data-aos-anchor="#example-anchor"
            data-aos-offset="500"
            data-aos-duration="500"
          >
            When you need to transport chilled or frozen products, <br />
            Petit Forestier offers a full range of vehicles for hire <br />
            on a short, medium or long-term basis.
          </p>
          <a href="#" id="__sdb">Download our brochure</a>
        </div>
      </div>
    </section>
    <section class="__LCamions">
      <div class="__CContainer">
        <h2 id="cch2">Our current range of vehicules</h2>
        <div class="__Camions">
          <div class="__Tc">
            <a
              id="__Cwr"
              href="#"
              data-aos="fade-up"
              class="__Trc"
              v-for="Camion in CamionsTc"
              :key="Camion"
            >
              <div class="__img">
                <img
                  id="_cwrimg"
                  :src="require(`../assets/Templtaes-NP/${Camion.img}`)"
                />
              </div>
              <div class="__Info" id="__cwrinfo">
                <h3 id="__cwrh3">
                  {{ Camion.name }} <br />
                  {{ Camion.pke }}
                </h3>
              </div>
            </a>
          </div>
          <div class="__Dc">
            <a
              id="__Cwr"
              href="#"
              data-aos="fade-left"
              class="__Trc"
              v-for="Camion in CamionsDc"
              :key="Camion"
            >
              <div class="__img">
                <img
                  id="_cwrimg"
                  :src="require(`../assets/Templtaes-NP/${Camion.img}`)"
                />
              </div>
              <div class="__Info" id="__cwrinfo">
                <h3 id="__cwrh3">
                  {{ Camion.name }} <br />
                  {{ Camion.pke }}
                </h3>
              </div>
            </a>
          </div>
        </div>
      </div>
    </section>
    <section class="__Work">
      <div class="__TStates" id="sta">
        <div id="_h2c_">
          <h2 id="__h2r" data-aos="fade-right">
            Working together <br />
            to ensure health & safety <br />
            and Food safety by simplifying <br />
            the cold chain every day.
          </h2>
        </div>

        <div
          id="__la"
          data-aos="fade-right"
          data-aos-offset="300"
          data-aos-easing="ease-in-sine"
        >
          <p class="__Green" id="__gr">
            Transport society, <br />
            world leader in refrigeration for hire
          </p>
          <p class="__THistory" id="__THr">
            Transport society is a family business, founded in France in 1907.
            <br />
            Through our knowledge and expertise, we have grown to become <br />
            the market leader in the cold storage sector. We have an extensive
            fleet <br />
            of hire vehicles at our disposal, across a large network of
            branches,
            <br />
            covering 22 countries in Europe, Middle-East, Africa <br />
            and in the USA. Through this coverage, Transport society serves over
            <br />
            15,000 customers, with a continued focus on providing high quality
            and
            <br />
            excellent service.
          </p>
          <br />
          <di class="__Mplus">
            <p class="Tsin" id="tsinm">Transport society in numbers</p>
            <div class="__Numbers">
              <div class="__div" id="__div">
                <div v-for="chiffre in Chiffres" :key="chiffre">
                  <p id="chm">
                    {{ chiffre.nbr }}
                  </p>
                  <p id="sjtm">
                    {{ chiffre.sjt }}
                  </p>
                </div>
              </div>
              <div class="__div" id="__div">
                <div v-for="chiffre in Chiffres01" :key="chiffre">
                  <p id="chm">
                    {{ chiffre.nbr }}
                  </p>
                  <p id="sjtm">
                    {{ chiffre.sjt }}
                  </p>
                </div>
              </div>
            </div>
          </di>
        </div>
      </div>
      <div
        data-aos="fade-left"
        data-aos-anchor="#example-anchor"
        data-aos-offset="500"
        data-aos-duration="500"
        class="__TConducteur"
        id="__tcr"
      >
        <img
          src="../assets/Templtaes-NP/AdobeStock_220195055.png"
          alt="Photo Conducteur de Camions"
        />
      </div>
    </section>
    <section class="__Specialist">
      <div class="__SpeContainer">
        <p class="__Sgreen" id="sgr">Transport society</p>
        <h2 id="__h2s">The refrigeration specialist</h2>
        <div class="__FlexCool" id="__FlexCool">
          <div
            data-aos="fade-up"
            data-aos-duration="3000"
            class="__Left"
            id="cool"
          >
            <div class="__TexAlignLeft">
              <p class="__Bolder" id="__br">
                The only 100% refrigerated <br />
                rental company
              </p>
              <p class="__Vide" id="__vr">
                Transport society is the only rental company <br />
                whose business focuses exclusively on cold <br />
                storage.
              </p>
            </div>
            <div class="__TexAlignLeft">
              <p class="__Bolder" id="__br">
                More than 100 years of expertise <br />
                in the transportation sector <br />
              </p>
              <p class="__Vide" id="__vr">
                Transport society hires out more than 5,500 <br />
                new refrigerated vehicles every year.
              </p>
            </div>
          </div>
          <div class="__Center">
            <img
              src="../assets/Templtaes-NP/Av_DobloFo.png"
              alt="Fourgon Doblon"
              width="600"
            />
          </div>
          <div
            data-aos="fade-down"
            data-aos-easing="linear"
            data-aos-duration="1500"
            class="__Right"
            id="cool"
          >
            <div class="__TexAlignRight">
              <p class="__Bolder" id="__br">+500 fridge specialist</p>
              <p class="__Vide" id="__vr">
                Trained to offer you the best in class service.
              </p>
            </div>
            <div class="__TexAlignRight">
              <p class="__Bolder" id="__br">Cemafroid accredited</p>
              <p class="__Vide" id="__vr">
                (ATP certifications) <br />
                Largest test centers network.
              </p>
            </div>
          </div>
        </div>
        <div class="__Manuf" id="manuf" data-aos="fade-left">
          <p class="__bolder" id="__br">Refrigerated body manufacturer</p>
          <p class="__Longer" id="__vr">
            2 manufacturing facilities for the design and manufacture of our
            refrigerated bodies. <br />
            Transport society is also an R&D department and a test laboratory to
            provide tailor-made <br />
            solutions to the specific needs of our customers and to design the
            refrigerated véhicles of <br />
            tomorrow.
          </p>
        </div>
      </div>
    </section>
    <section class="__Mecano" id="__meca">
      <div
        class="__img"
        id="__img"
        data-aos="fade-zoom-in"
        data-aos-easing="ease-in-back"
        data-aos-delay="300"
        data-aos-offset="0"
      >
        <img
          src="../assets/Templtaes-NP/Mécanicien.png"
          alt="Photo d'un Mécanicien"
          width="600"
        />
      </div>
      <div class="__Service" id="__service" data-aos="fade-right">
        <h2 id="__fsr">Full service !</h2>
        <div class="__FullS" id="_egap">
          <div class="__2s" id="fs">
            <div
              class="__OS"
              id="os"
              v-for="service in services01"
              :key="service"
            >
              <p class="__bolder" id="__br">
                {{ service.nbr }}
              </p>
              <p class="__lower" id="__vr">
                {{ service.sjt }}
              </p>
            </div>
          </div>
          <div class="__2s" id="fs">
            <div
              class="__OS"
              id="os"
              v-for="service in services02"
              :key="service"
            >
              <p class="__bolder" id="__br">
                {{ service.nbr }}
              </p>
              <p class="__lower" id="__vr">
                {{ service.sjt }}
              </p>
            </div>
          </div>
        </div>
        <a href="#" id="_sd">Download our brochure</a>
      </div>
    </section>
    <section class="__contact" id="contact">
      <div class="__contactContainer" id="cc__">
        <div class="__info" id="__info">
          <h2 id="__dnr">Contact us</h2>
          <img id="__ci" src="../assets/Templtaes-NP/Bitmap.png" width="450" />
          <p class="__Itext" id="itext">
            For more information, please don’t <br />
            hesitate to get in touch with William :
          </p>
          <p class="_Mul" id="mul">
            William Racinne – Country Director <br />
            Telephone: +27 72 134 1225 <br />
            Email : wracinne@transportsociety.co.za <br />
            Twitter : @WilliamRacinne
          </p>
        </div>
        <form class="__form" data-aos="fade-left">
          <div class="__profileTitle">
            <div class="__profile">
              <p class="__bolder">Profile</p>
              <div class="__radio">
                <div>
                  <input
                    type="radio"
                    id="Consumer."
                    name="person"
                    value="Consumer."
                    checked
                  />
                  <label for="Consumer.">Consumer.</label><br />
                </div>
                <div>
                  <input
                    type="radio"
                    id="Professionnal"
                    name="person"
                    value="Professionnal"
                  />
                  <label for="Professionnal">Professionnal</label><br />
                </div>
              </div>
            </div>
            <div class="__title">
              <p class="__bolder">Title</p>
              <div class="__radio">
                <div>
                  <input type="radio" id="M" name="gen" value="30" checked />
                  <label for="M">M.</label>
                </div>
                <div>
                  <input type="radio" id="Mrs." name="gen" value="60" />
                  <label for="Mrs.">Mrs.</label>
                </div>
              </div>
            </div>
          </div>
          <div class="__fullName">
            <div class="__Forename">
              <label for="Forename">Forename</label>
              <input type="text" id="Forename" />
            </div>
            <div class="__Surmame">
              <label for="Surmame">Surmame</label>
              <input type="text" id="Surmame" />
            </div>
          </div>
          <div class="__reason">
            <div class="__Forename">
              <label for="Forename">Company name</label>
              <input type="text" id="Forename" />
            </div>
            <div class="__Surmame">
              <label for="Surmame">Job title</label>
              <input type="text" id="Surmame" />
            </div>
          </div>
          <div class="__email">
            <div class="__Forename">
              <label for="Forename">Email adress</label>
              <input type="email" id="Forename" />
            </div>
          </div>
          <div class="__Phone">
            <div class="__Forename">
              <label for="Forename">Telephone</label>
              <input type="text" id="Forename" />
            </div>
            <div class="__Surmame">
              <label for="Surmame">Country</label>
              <select name="pets" id="Cselect">
                <option value="South Africa">South Africa</option>
                <option value="GE">Georgia</option>
                <option value="DE">Germany</option>
              </select>
            </div>
          </div>
          <div class="__message">
            <div class="__Forename">
              <label for="Forename">Email adress</label>
              <textarea
                name="msg"
                id="msg"
                cols="30"
                rows="10"
                placeholder="Your message"
              />
            </div>
          </div>
          <div class="__conditions">
            <div class="__chart">
              <input type="checkbox" id="chk" />
              <label for="chk"
                >Cochez cette case si, au-delà de la réponse à votre demande
                d'information, vous souhaitez <br />
                recevoir d'autres communications de notre part.*</label
              >
            </div>

            <button type="submit">Submit</button>
          </div>
        </form>
      </div>
    </section>
    <section class="__maps">
      <div class="__locInfo">
        <div class="__loc __Important">
          <p class="__title __bolder">Our agencies in South Africa</p>
          <p class="__info __address">
            Contact : Jacobus Van Niekerk <br />
            Telephone: +27 67 674 0573
          </p>
        </div>
        <hr />
        <a
          href="https://goo.gl/maps/M9mGx5RY9FPppZTQ7"
          target="_blank"
          class="__loc"
        >
          <i class="fa-solid fa-angle-right"></i>
          <p class="__bolder">Johannesburg</p>
          <p class="__address">
            99 Skew Road, 1459, <br />
            Boksburg, Gauteng
          </p>
        </a>
        <hr />
        <a
          href="https://goo.gl/maps/M9mGx5RY9FPppZTQ7"
          target="_blank"
          class="__loc"
        >
          <i class="fa-solid fa-angle-right"></i>
          <p class="__bolder">Durban</p>
          <p class="__address">
            Unit 4b, 50 Moreland Drive, Rinaldo Industrial Park,<br />
            Redhill 4071, Durban, KZN
          </p>
        </a>
        <hr />
        <a
          href="https://goo.gl/maps/M9mGx5RY9FPppZTQ7"
          target="_blank"
          class="__loc"
        >
          <i class="fa-solid fa-angle-right"></i>
          <p class="__bolder">Cape Town</p>
          <p class="__address">
            111 Kruis Road, Brackenfell, <br />
            7560, Cape Town, Western Cape
          </p>
        </a>
      </div>
      <iframe
        src="https://my.atlistmaps.com/map/a5f0f764-5f2b-4138-b41c-82f50cfa20e8?share=true"
        allow="geolocation"
        width="100%"
        height="400px"
        frameborder="0"
        scrolling="no"
        allowfullscreen
      ></iframe>
    </section>
    <footer>
      <section class="__copywright">
        <a href="#" class="__logoFooter">
          <img
            src="../assets/Templtaes-NP/logo.png"
            alt="Logo Transport Society"
            title="Logo Transport Society"
            width="80"
          />
          <div class="__LogoTextFooter">
            Transport <br />
            Society
          </div>
        </a>
        <div
          class="__txt"
          data-aos="fade-up"
          data-aos-anchor-placement="center-bottom"
        >
          <p class="__top">
            *Les informations que nous collections via ce formulaire font
            l’objet d’un traitement informatique dont la finalité est de pouvoir
            répondre à votre demande d'information.
          </p>
          <p class="__center">
            Les destinataires des données sont les services marketing et
            commercial du groupe Transport society <br />
            Conformément à la loi du 6 janvier 1978 relative à l'infromatique,
            aux fichiers et aux libertés modifiée par la loi du 20 juin 2018 et
            au Règlement de l'Union européenne n°2016/679 relatif à <br />
            la protection des personnes physiques à l'égard du traitement des
            données à caractère personnel et à la libre circulation des données
            (RGPD), vous disposez d'un droit d'accès, <br />
            de rectification, de limitation, d'opposition, de portabilité, de
            limitation et d'effacement des informations qui vous concernent - en
            envoyant un courrier à dpo@transportsociety.com <br />
            accompagné d'une copie d'une pièce d'identité valide.
          </p>
          <p class="__bottom">
            En soumettant ce formulaire, vous acceptez notre politique de
            confidentialité.
          </p>
        </div>
      </section>
      <section class="__enfin">
        <p>Legal notice</p>
        <p>private policy</p>
        <p>© 2022 Transport society</p>
      </section>
    </footer>
  </div>
</template>

<script>
import { ref, onMounted } from "vue";

//...
export default {
  setup() {
    const CamionsTc = ref([
      {
        name: "UD Trucks Croner",
        pke: " PKE250 H30",
        img: "UD-Trucks-Croner.png",
      },
      {
        name: "Isuzu FTR 850",
        img: "Isuzu FTR 850.png",
      },
      {
        name: "Isuzu NQR 500",
        img: "Isuzu NQR 500.png",
      },
    ]);
    //...
    const CamionsDc = ref([
      {
        name: "Toyota Dyna",
        img: "Toyota Dyna.png",
      },
      {
        name: "Fiat Doblo fourgon",
        img: "Fiat Doblo fourgon.png",
      },
    ]);
    //...
    const Chiffres = ref([
      {
        nbr: "+62,000",
        sjt: "refrigerated vehicles",
      },
      {
        nbr: "+15 000",
        sjt: "customers",
      },
      {
        nbr: "+4,500",
        sjt: "employees",
      },
    ]);
    //...
    const Chiffres01 = ref([
      {
        nbr: "+300",
        sjt: "sites worldwide",
      },
      {
        nbr: "€849 M",
        sjt: "turnover in 2021",
      },
      {
        nbr: "500+",
        sjt: "refrigeration specialists",
      },
    ]);
    //...
    const services01 = ref([
      {
        nbr: "24/7 support",
        sjt: "Round-the-clock assistance, every day, 365 days a year. Provision of a replacement refrigerated vehicle in the event of a breakdown.",
      },
      {
        nbr: "Spare parts",
        sjt: "Provision of tyres, fluids and lubricants.",
      },
      {
        nbr: "Administrative support",
        sjt: "We take care of all administrative procedures: license renewal, test certificates, legal paperwork.",
      },
    ]);
    //...
    const services02 = ref([
      {
        nbr: "Maintenance",
        sjt: "We carry out legally required tests and preventive maintenance on the vehicles and their equipments.",
      },
      {
        nbr: "Repairs",
        sjt: "Repairs to the bodywork and paintwork, as well as all mechanical repairs.",
      },
      {
        nbr: "Customisation",
        sjt: "Your vehicle can be customized with your own livery.",
      },
    ]);
    //...
    function toggle() {
      const toggleitem = document.querySelector(".__toggle");
      toggleitem.classList.add("__descend");
    }
    function toggleUp() {
      const toggleitem = document.querySelector(".__toggle");
      toggleitem.classList.remove("__descend");
    }
    //...
    onMounted(function () {
      AOS.init();
    });
    //...
    return {
      CamionsTc,
      CamionsDc,
      Chiffres,
      Chiffres01,
      services01,
      services02,
      toggle,
      toggleUp,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url(https://fonts.googleapis.com/css?family=Poppins:100,100italic,200,200italic,300,300italic,regular,italic,500,500italic,600,600italic,700,700italic,800,800italic,900,900italic);
@import url(https://fonts.googleapis.com/css?family=Mulish:200,300,regular,500,600,700,800,900,200italic,300italic,italic,500italic,600italic,700italic,800italic,900italic);
:root {
  --flex-: {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
}

hr {
  margin: 0;
  opacity: 30%;
}

.__HomeScreen {
  overflow: hidden;
}

.__HomeScreen .__toggle {
  display: none;
}

.__HomeScreen .__Header {
  height: 100px;
  padding: 0 2rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Header .__Logo {
  text-decoration: none;
  color: black;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Header .__Logo .__LogoText {
  font-weight: bold;
  text-align: left;
}

.__HomeScreen .__Header .__Nav {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  height: 100%;
}

.__HomeScreen .__Header .__Nav li {
  height: 100%;
  list-style: none;
  margin: 0 1rem;
  font-weight: 600;
  -webkit-transition: 0.5s linear;
  transition: 0.5s linear;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Header .__Nav li a {
  padding: 0 0.5rem;
  text-decoration: none;
  color: black;
  height: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Header .__Nav li:hover {
  background-color: #039f4e;
}

.__HomeScreen .__Header .__Nav li:hover a {
  color: white;
}

.__HomeScreen .__Header .__Nav .__Region {
  height: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 1rem;
  margin: 0 0 0 2rem;
  font-weight: 600;
  -webkit-transition: 300ms;
  transition: 300ms;
  position: relative;
  cursor: pointer;
}

.__HomeScreen .__Header .__Nav .__Region .__Safrica {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 0.6rem;
}

.__HomeScreen .__Header .__Nav .__Region .__Safrica i {
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.__HomeScreen .__Header .__Nav .__Region:hover .__Safrica i {
  -webkit-transform: rotate(180deg);
  transform: rotate(180deg);
}

.__HomeScreen .__Header .fa-align-right {
  display: none;
  margin: 0 2rem 0 0;
  font-size: 2rem;
  cursor: pointer;
}

.__HomeScreen .__SauteOYeux {
  margin: 0;
  height: 70vh;
  background: url("../assets/Banner.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: right;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__SauteOYeux .__PresentationContainer {
  height: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__SauteOYeux .__PresentationContainer div {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  text-align: left;
  width: -webkit-max-content;
  width: -moz-max-content;
  width: max-content;
  height: 20rem;
  margin-left: 2rem;
  color: white;
}

.__HomeScreen .__SauteOYeux .__PresentationContainer div h1 {
  font-size: 48px;
  font-weight: bold;
  margin: 0;
  padding: 0;
  height: -webkit-min-content;
  height: -moz-min-content;
  height: min-content;
}

.__HomeScreen .__SauteOYeux .__PresentationContainer div p,
.__HomeScreen .__SauteOYeux .__PresentationContainer div a {
  font-family: Mulish;
  font-size: 18px;
  margin: 0;
}

.__HomeScreen .__SauteOYeux .__PresentationContainer div a {
  background-color: #fff;
  color: black;
  padding: 1rem 2rem;
  font-weight: 700;
  text-decoration: none;
}

.__HomeScreen .__LCamions {
  padding: 3rem 0;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__LCamions .__CContainer {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__LCamions .__CContainer h2 {
  font-size: 2rem;
}

.__HomeScreen .__LCamions .__CContainer .__Camions {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 4rem;
}

.__HomeScreen .__LCamions .__CContainer .__Camions .__Tc,
.__HomeScreen .__LCamions .__CContainer .__Camions .__Dc {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__LCamions .__CContainer .__Camions .__Tc .__Trc,
.__HomeScreen .__LCamions .__CContainer .__Camions .__Dc .__Trc {
  text-decoration: none;
  width: 325px;
  border-radius: 10px;
  overflow: hidden;
  margin: 0 2rem;
  -webkit-box-shadow: #959da533 0px 8px 24px;
  box-shadow: #959da533 0px 8px 24px;
}

.__HomeScreen .__LCamions .__CContainer .__Camions .__Tc .__Trc .__img,
.__HomeScreen .__LCamions .__CContainer .__Camions .__Dc .__Trc .__img {
  background-color: #039f4e;
  height: 147px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__LCamions .__CContainer .__Camions .__Tc .__Trc .__Info,
.__HomeScreen .__LCamions .__CContainer .__Camions .__Dc .__Trc .__Info {
  height: 86px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__LCamions .__CContainer .__Camions .__Tc .__Trc .__Info h3,
.__HomeScreen .__LCamions .__CContainer .__Camions .__Dc .__Trc .__Info h3 {
  margin: 0 1rem;
  color: black;
}

.__HomeScreen .__Work {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  padding: 2rem;
}

.__HomeScreen .__Work .__TStates {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__Work .__TStates h2 {
  font-size: 40px;
  margin: 0;
}

.__HomeScreen .__Work .__TStates .__Green {
  color: #039f4e;
  font-weight: bold;
  font-size: 20px;
}

.__HomeScreen .__Work .__TStates .__THistory {
  font-family: Mulish, sans-serif;
  margin-top: 0;
}

.__HomeScreen .__Work .__TStates .__Mplus .Tsin {
  color: #039f4e;
  font-weight: bold;
  font-size: 20px;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  gap: 2rem;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers .__div {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  -ms-flex-direction: row;
  flex-direction: row;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 2rem;
  font-family: Mulish, sans-serif;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers .__div div {
  width: 12rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers .__div div p {
  margin: 0;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers .__div div p:nth-child(1) {
  font-size: 25px;
}

.__HomeScreen .__Work .__TStates .__Mplus .__Numbers .__div div p:nth-child(2) {
  color: #7b7d7c;
  font-size: 16px;
}

.__HomeScreen .__Work .__TConducteur {
  height: inherit;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: start;
}

.__HomeScreen .__Work .__TConducteur img {
  border-radius: 10px;
}

.__HomeScreen .__Specialist {
  padding: 2rem 0;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  padding-top: 4rem;
  padding-bottom: 4rem;
}

.__HomeScreen .__Specialist .__SpeContainer {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Specialist .__SpeContainer .__Sgreen {
  font-size: 20px;
  font-weight: bold;
  color: #00a343;
}

.__HomeScreen .__Specialist .__SpeContainer h2 {
  font-size: 40px;
  margin: 0;
}

.__HomeScreen .__Specialist .__SpeContainer .__FlexCool {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  margin-top: 3rem;
}

.__HomeScreen .__Specialist .__SpeContainer .__FlexCool .__Left {
  height: 414px;
  width: 357px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Left
  .__TexAlignLeft {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: end;
  -ms-flex-align: end;
  align-items: flex-end;
  width: 100%;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Left
  .__TexAlignLeft
  .__Bolder {
  text-align: right;
  font-weight: bold;
  font-size: 18px;
  margin: 0;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Left
  .__TexAlignLeft
  .__Vide {
  font-size: 16px;
  text-align: right;
}

.__HomeScreen .__Specialist .__SpeContainer .__FlexCool .__Right {
  height: 414px;
  width: 357px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Right
  .__TexAlignRight {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  width: 100%;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Right
  .__TexAlignRight
  .__Bolder {
  margin: 0;
  text-align: left;
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__Specialist
  .__SpeContainer
  .__FlexCool
  .__Right
  .__TexAlignRight
  .__Vide {
  font-size: 16px;
  text-align: left;
}

.__HomeScreen .__Specialist .__SpeContainer .__Manuf {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  margin-top: 2rem;
}

.__HomeScreen .__Specialist .__SpeContainer .__Manuf .__bolder {
  font-size: 18px;
  font-weight: bold;
}

.__HomeScreen .__Specialist .__SpeContainer .__Manuf .__Longer {
  font-size: 15px;
  text-align: center;
  margin: 0;
}

.__HomeScreen .__Mecano {
  overflow: hidden;
  background: url("../assets/FULL SERVICE.png");
  background-size: cover;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__Mecano .__img {
  -webkit-transform: translateY(0.5rem);
  transform: translateY(0.5rem);
}

.__HomeScreen .__Mecano .__Service {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  color: white;
  margin-right: 10rem;
  margin-top: 3rem;
}

.__HomeScreen .__Mecano .__Service h2 {
  font-size: 40px;
}

.__HomeScreen .__Mecano .__Service .__FullS {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 2rem;
  font-family: Mulish, sans-serif;
  height: 350px;
}

.__HomeScreen .__Mecano .__Service .__FullS .__2s {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  gap: 2rem;
  width: 305px;
  height: 360px;
}

.__HomeScreen .__Mecano .__Service .__FullS .__2s .__OS {
  height: 126px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__Mecano .__Service .__FullS .__2s .__OS .__bolder {
  font-size: 20px;
  font-weight: bold;
  margin: 0;
}

.__HomeScreen .__Mecano .__Service .__FullS .__2s .__OS .__lower {
  margin: 0;
  font-size: 16px;
}

.__HomeScreen .__Mecano .__Service a {
  text-decoration: none;
  color: black;
  background-color: #fff;
  margin-top: 3rem;
  padding: 1rem 2rem;
  font-family: Mulish, sans-serif;
  font-weight: bold;
}

.__HomeScreen .__contact {
  padding: 3rem 0;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  margin: 0 2rem;
  width: 100%;
  height: 90%;
}

.__HomeScreen .__contact .__contactContainer .__info {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__contact .__contactContainer .__info h2 {
  font-size: 40px;
  margin-top: 0;
}

.__HomeScreen .__contact .__contactContainer .__info .__Itext {
  font-weight: bold;
  font-size: 20px;
  margin-bottom: 0;
}

.__HomeScreen .__contact .__contactContainer .__info ._Mul {
  font-family: Mulish, sans-serif;
  font-size: 18px;
}

.__HomeScreen .__contact .__contactContainer .__form {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 1.4rem;
}

.__HomeScreen .__contact .__contactContainer .__form .__profileTitle {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 2rem;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__profile {
  width: 290px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__profile
  .__bolder {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__profile
  .__radio {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  gap: 2.4rem;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__profile
  .__radio
  div {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 0.3rem;
}

.__HomeScreen .__contact .__contactContainer .__form .__profileTitle .__title {
  width: 290px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__title
  .__bolder {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__title
  .__radio {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  gap: 2.4rem;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__profileTitle
  .__title
  .__radio
  div {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 0.3rem;
}

.__HomeScreen .__contact .__contactContainer .__form .__fullName {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer .__form .__fullName .__Forename {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Forename
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Forename
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Forename
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__fullName .__Surmame {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Surmame
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Surmame
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__fullName
  .__Surmame
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__reason {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer .__form .__reason .__Forename {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Forename
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Forename
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Forename
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__reason .__Surmame {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Surmame
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Surmame
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__reason
  .__Surmame
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__email {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer .__form .__email .__Forename {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__email
  .__Forename
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__email
  .__Forename
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__email
  .__Forename
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__Phone {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer .__form .__Phone .__Forename {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Forename
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Forename
  input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Forename
  input:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__Phone .__Surmame {
  width: 290px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen .__contact .__contactContainer .__form .__Phone .__Surmame label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen .__contact .__contactContainer .__form .__Phone .__Surmame input {
  height: 2rem;
  border: none;
  text-align: center;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Surmame
  input:focus {
  outline: none;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Surmame
  select {
  border: none;
  height: 2rem;
  border: none;
  border-bottom: 2px solid #a5a5a5;
  outline: none;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__Phone
  .__Surmame
  select
  option {
  padding: 2rem;
}

.__HomeScreen .__contact .__contactContainer .__form .__message {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__contact .__contactContainer .__form .__message .__Forename {
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__message
  .__Forename
  label {
  font-weight: bold;
  font-size: 18px;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__message
  .__Forename
  textarea {
  max-height: 2rem;
  min-width: 100%;
  border: none;
  border-bottom: 2px solid #a5a5a5;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__message
  .__Forename
  textarea:focus {
  outline: none;
}

.__HomeScreen .__contact .__contactContainer .__form .__conditions {
  margin-top: 1.5rem;
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__contact .__contactContainer .__form .__conditions .__chart {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  gap: 4px;
  cursor: pointer;
}

.__HomeScreen
  .__contact
  .__contactContainer
  .__form
  .__conditions
  .__chart
  input {
  -webkit-transform: translateY(3px);
  transform: translateY(3px);
}

.__HomeScreen .__contact .__contactContainer .__form .__conditions button {
  margin: 3rem 0 0 0;
  background-color: #00a343;
  color: white;
  padding: 1rem 9rem;
  border: none;
  cursor: pointer;
}

.__HomeScreen .__maps {
  position: relative;
}

.__HomeScreen .__maps iframe {
  height: 100vh;
  width: 100%;
}

.__HomeScreen .__maps .__locInfo {
  position: absolute;
  top: 3rem;
  left: 2rem;
  margin-right: 2rem;
}

.__HomeScreen .__maps .__locInfo .__loc {
  text-decoration: none;
  color: black;
  background-color: #ffffff;
  padding: 1rem 5rem 1rem 1rem;
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
}

.__HomeScreen .__maps .__locInfo .__loc i {
  position: absolute;
  right: 2rem;
}

.__HomeScreen .__maps .__locInfo .__loc .__bolder {
  font-size: 20px;
  font-weight: bold;
  margin: 0 0 0.5rem 0;
}

.__HomeScreen .__maps .__locInfo .__loc .__address {
  margin: 0;
  font-size: 15px;
  font-family: Mulish, sans-serif;
}

.__HomeScreen .__maps .__locInfo .__Important {
  background-color: #f3f3f3;
}

.__HomeScreen .__maps .__locInfo .__Important .__title {
  margin: 0;
}

.__HomeScreen .__maps .__locInfo .__Important .__info {
  margin: 0;
}

.__HomeScreen .__maps .__locInfo .__Important .__bolder {
  margin-bottom: 0.6rem;
}

.__HomeScreen .__copywright {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: space-evenly;
  -ms-flex-pack: space-evenly;
  justify-content: space-evenly;
  -webkit-box-align: start;
  -ms-flex-align: start;
  align-items: flex-start;
  padding: 2rem;
}

.__HomeScreen .__copywright .__logoFooter {
  margin: 1rem 1rem 0 0;
  text-decoration: none;
  color: black;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  -ms-flex-direction: column;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
}

.__HomeScreen .__copywright .__logoFooter .__LogoTextFooter {
  font-weight: bold;
  text-align: left;
  font-size: 18px;
}

.__HomeScreen .__copywright .__txt {
  font-size: 12px;
}

.__HomeScreen .__enfin {
  color: white;
  background-color: black;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: start;
  -ms-flex-pack: start;
  justify-content: flex-start;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  gap: 3rem;
  height: 90px;
  padding-left: 2rem;
  font-size: 16px;
}

@media only screen and (max-width: 1450px) {
  .__HomeScreen {
    position: relative;
  }
  .__HomeScreen #__ci {
    width: 290px;
  }
  .__HomeScreen .__toggle {
    -webkit-transition: 0.9s cubic-bezier(1, 0, 0, 1);
    transition: 0.9s cubic-bezier(1, 0, 0, 1);
    -webkit-transform: translateY(-100vh);
    transform: translateY(-100vh);
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    position: fixed;
    z-index: 1;
    height: 20rem;
    width: 100%;
    background-color: white;
  }
  .__HomeScreen .__toggle .__Nav {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    height: 30%;
  }
  .__HomeScreen .__toggle .__Nav li {
    height: 100%;
    list-style: none;
    margin: 0 2rem;
    font-weight: 600;
    -webkit-transition: 0.5s linear;
    transition: 0.5s linear;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .__HomeScreen .__toggle .__Nav li a {
    padding: 0 0.5rem;
    text-decoration: none;
    color: black;
    height: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .__HomeScreen .__toggle .__Nav li:hover {
    background-color: #039f4e;
  }
  .__HomeScreen .__toggle .__Nav li:hover a {
    color: white;
  }
  .__HomeScreen .__toggle .__Nav .__Region {
    height: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    gap: 1rem;
    margin: 0 0 0 2rem;
    font-weight: 600;
    -webkit-transition: 300ms;
    transition: 300ms;
    position: relative;
    cursor: pointer;
  }
  .__HomeScreen .__toggle .__Nav .__Region .__Safrica {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    gap: 0.6rem;
  }
  .__HomeScreen .__toggle .__Nav .__Region .__Safrica i {
    -webkit-transition: 0.4s;
    transition: 0.4s;
  }
  .__HomeScreen .__toggle .__Nav .__Region:hover .__Safrica i {
    -webkit-transform: rotate(180deg);
    transform: rotate(180deg);
  }
  .__HomeScreen .__toggle .fa-xmark {
    position: absolute;
    top: 2rem;
    right: 2rem;
    font-size: 2rem;
    cursor: pointer;
  }
  .__HomeScreen .__descend {
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  .__HomeScreen .__Header {
    padding: 0;
  }
  .__HomeScreen .__Header .__Logo {
    margin-left: 2rem;
  }
  .__HomeScreen .__Header .__Nav {
    display: none;
  }
  .__HomeScreen .__Header .fa-align-right {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  .__HomeScreen .__PresentationContainer #__soyt {
    -ms-flex-pack: distribute;
    justify-content: space-around;
  }
  .__HomeScreen .__PresentationContainer #__soyt #__h1r {
    font-size: 39px;
    margin-bottom: 0;
  }
  .__HomeScreen .__PresentationContainer #__soyt .__p1r {
    font-size: 15px;
    margin: 0;
  }
  .__HomeScreen .__LCamions #__Cwr {
    width: 295px;
  }
  .__HomeScreen .__Work #__h2r {
    font-size: 30px;
  }
  .__HomeScreen .__Work #__gr {
    font-size: 17px;
  }
  .__HomeScreen .__Work #__THr {
    font-size: 14px;
  }
  .__HomeScreen .__Work .__Mplus #tsinm {
    font-size: 17px;
  }
  .__HomeScreen .__Work .__Mplus #chm {
    font-size: 20px;
  }
  .__HomeScreen .__Work .__Mplus #sjtm {
    font-size: 13px;
  }
  .__HomeScreen .__Specialist #sgr {
    font-size: 15px;
  }
  .__HomeScreen .__Specialist #__h2s {
    font-size: 32px;
  }
  .__HomeScreen .__Specialist #__br {
    font-size: 13px;
  }
  .__HomeScreen .__Specialist #__vr {
    font-size: 12px;
  }
  .__HomeScreen .__Mecano #__service {
    margin-right: 8vh;
  }
  .__HomeScreen .__Mecano #__fsr {
    font-size: 35px;
  }
  .__HomeScreen .__Mecano #__br {
    font-size: 16px;
  }
  .__HomeScreen .__Mecano #__vr {
    font-size: 14px;
  }
}

@media only screen and (max-width: 1380px) {
  .__Center img {
    width: 500px;
  }
  #__SauteOYeux {
    height: 70vh;
  }
  #__h2r {
    text-align: right;
    font-size: 20px !important;
  }
  .__Work {
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .__Work #_h2c_ {
    height: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: end;
    -ms-flex-pack: end;
    justify-content: flex-end;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .__Work #__tcr {
    display: none;
  }
  .__Work #sta {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-direction: row;
    flex-direction: row;
    -webkit-box-pack: space-evenly;
    -ms-flex-pack: space-evenly;
    justify-content: space-evenly;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    width: 100%;
    height: 100%;
  }
  .__Work #sta #__la {
    width: 500px;
  }
  .__Work #sta #__la #__gr {
    font-size: 12px;
  }
  .__Work #sta #__la #__THr {
    font-size: 12px;
  }
  .__Work #sta #__la #tsinm {
    font-size: 14px;
  }
  .__Work #sta #__la #chm {
    font-size: 17px;
  }
  .__Work #sta #__la #__div {
    gap: 0;
  }
  #__meca {
    padding: 2rem 0;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  #__meca #__img {
    display: none;
  }
  #__meca #__service {
    margin-left: 20rem;
  }
  #contact #cc__ {
    height: -webkit-max-content;
    height: -moz-max-content;
    height: max-content;
    -webkit-box-orient: vertical;
    -webkit-box-direction: reverse;
    -ms-flex-direction: column-reverse;
    flex-direction: column-reverse;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  #contact #cc__ #__info {
    width: 100%;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
    gap: 1rem;
    height: 100%;
  }
  #contact #cc__ #__info #__ci {
    display: none;
  }
  #contact #cc__ #__info #itext {
    text-align: right;
  }
  #contact #cc__ #__info #mul {
    text-align: right;
  }
  #contact #cc__ #__info #__dnr {
    display: none;
  }
}

@media only screen and (max-width: 1300px) {
  #__SauteOYeux {
    height: -webkit-max-content;
    height: -moz-max-content;
    height: max-content;
    padding: 2rem 0;
  }
  .__Center img {
    width: 300px;
  }
  #__FlexCool {
    margin-top: 0;
  }
  #__FlexCool #cool {
    margin: 1rem 0;
    height: 250px;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
  }
  #manuf {
    margin-top: 0;
  }
  .__enfin p {
    font-size: 10px !important;
  }
  #__h2s {
    font-size: 25px !important;
  }
}

@media only screen and (max-width: 1116px) {
  #__meca {
    padding: 0 0 2rem 0;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: end;
    -ms-flex-pack: end;
    justify-content: flex-end;
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
  }
  #__meca #__service {
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
    text-align: right;
  }
  #__meca #__service #os {
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
    height: -webkit-max-content;
    height: -moz-max-content;
    height: max-content;
  }
  #__meca #__service #_egap {
    gap: 0;
    height: -webkit-max-content;
    height: -moz-max-content;
    height: max-content;
  }
  #__meca #__service #fs {
    -webkit-box-align: end;
    -ms-flex-align: end;
    align-items: flex-end;
    height: 305px;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
  }
  #__meca #__fsr {
    font-size: 30px;
    margin-bottom: 0;
  }
  #__meca #__br {
    font-size: 13px;
  }
  #__meca #__vr {
    font-size: 11px;
  }
}

@media only screen and (max-width: 1100px) {
  .__LCamions #cch2 {
    font-size: 23px;
  }
  .__LCamions #__Cwr {
    width: 205px !important;
    height: 200px;
  }
  .__LCamions #__Cwr #_cwrimg {
    width: 140px;
  }
  .__LCamions #__Cwr #__cwrinfo {
    height: -webkit-max-content;
    height: -moz-max-content;
    height: max-content;
  }
  .__LCamions #__Cwr #__cwrinfo #__cwrh3 {
    font-size: 16px;
  }
  .__PresentationContainer #__soyt #__h1r {
    font-size: 32px !important;
    margin-bottom: 0;
  }
  .__PresentationContainer #__soyt .__p1r {
    font-size: 11px !important;
    margin: 0;
  }
  .__PresentationContainer #__sdb {
    padding: 0.5rem 1rem;
  }
  #sta #__la {
    width: 380px !important;
  }
  #sta #__la #__gr {
    font-size: 12px;
  }
  #sta #__la #__THr {
    font-size: 12px;
  }
  #sta #__la #tsinm {
    font-size: 14px;
  }
  #sta #__la #chm {
    font-size: 17px;
  }
  #sta #__la #__div {
    gap: 0;
  }
  #sta #__la #__div div {
    width: 8rem !important;
  }
  #_sd {
    margin-top: 0;
  }
}

@media only screen and (max-width: 900px) {
  #__SauteOYeux {
    padding: 0;
    background: url("../assets/Bitmap.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: right;
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  #__SauteOYeux #__PresentationContainer {
    padding: 2rem 0;
    height: 100%;
    width: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -webkit-backdrop-filter: blur(6px);
    backdrop-filter: blur(6px);
  }

  .__HomeScreen .__Mecano .__Service {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: start;
    -ms-flex-align: start;
    align-items: flex-start;
    color: white;
    margin: 3rem 1rem 0 1rem !important;
  }
  .__HomeScreen .__Work {
    justify-content: center !important;
    padding: 0 !important;
  }
  .__Work #sta #__la {
    width: min-content !important;
    display: -webkit-box !important;
    display: -ms-flexbox !important;
    display: flex !important;
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
    -webkit-box-pack: center !important;
    -ms-flex-pack: center !important;
    justify-content: center !important;
  }
  .__Work #sta #__la #tsinm {
  width: 100% ;
  }
  .__Work #sta #__la .__Mplus {
    display: -webkit-box !important;
    display: -ms-flexbox !important;
    display: flex !important;
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
    -webkit-box-pack: center !important;
    -ms-flex-pack: center !important;
    justify-content: center !important;
    -webkit-box-align: center !important;
    -ms-flex-align: center !important;
    align-items: center !important;
  }
  #sta #__la #__div div {
    width: 6rem !important;
    #chm {
      font-size: 14px !important;
    }
    #sjtm {
      font-size: 11px !important;
    }
  }
  /* ___ */
  .__CContainer {
    width: 65% !important;
  }
  .__Camions {
    gap: 1rem !important;
    width: 100% !important;
  }
  .__Camions .__Tc,
  .__Camions .__Dc {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    gap: 1rem;
    width: 100% !important;
  }
  .__Camions .__Tc #__Cwr,
  .__Camions .__Dc #__Cwr {
    width: 100% !important;
  }
  .__Work .__TStates {
    padding: 0 1rem !important;
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
  }
  .__Work .__TStates #__h2r {
    font-size: 17px !important;
  }
  .__Work .__TStates #__THr {
    font-size: 8px !important;
  }
  .__toggle {
    height: 100vh !important;
  }
  .__toggle .__Nav {
    height: -webkit-max-content !important;
    height: -moz-max-content !important;
    height: max-content !important;
    display: -webkit-box !important;
    display: -ms-flexbox !important;
    display: flex !important;
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
    -webkit-box-pack: center !important;
    -ms-flex-pack: center !important;
    justify-content: center !important;
    -webkit-box-align: center !important;
    -ms-flex-align: center !important;
    align-items: center !important;
    gap: 1rem !important;
  }
  .__toggle .__Nav li {
    height: 2rem !important;
  }
  .__toggle .__Nav li a {
    height: 100% !important;
  }
  .__FlexCool {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .__Center {
    display: none !important;
  }
  #__h2s {
    text-align: center !important;
  }
  .__TexAlignLeft,
  .__TexAlignRight {
    -webkit-box-align: center !important;
    -ms-flex-align: center !important;
    align-items: center !important;
  }
  .__TexAlignLeft .__Bolder,
  .__TexAlignLeft .__Vide,
  .__TexAlignRight .__Bolder,
  .__TexAlignRight .__Vide {
    text-align: center !important;
  }
  #manuf {
    padding: 0 1rem;
  }
  #cool {
    -ms-flex-pack: distribute !important;
    justify-content: space-around !important;
    margin: 0 1rem !important;
  }
  .__Mecano {
    background: #00a343 !important;
  }
  .__Mecano .__FullS {
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
  }
  .__Mecano .__FullS #fs {
    height: 214px !important;
  }
  .__form label {
    font-size: 14px !important;
  }
  .__form .__profileTitle {
    flex-direction: column !important;
    width: 290px !important;
  }
  .__form .__profileTitle .__profile .__radio,
  .__form .__profileTitle .__title .__radio {
    gap: 0 !important;
  }
  .__form .__fullName,
  .__form .__reason,
  .__form .__Phone {
    -webkit-box-orient: vertical !important;
    -webkit-box-direction: normal !important;
    -ms-flex-direction: column !important;
    flex-direction: column !important;
  }
  .__form .__email,
  .__form .__message {
    display: -webkit-box !important;
    display: -ms-flexbox !important;
    display: flex !important;
    -webkit-box-pack: center !important;
    -ms-flex-pack: center !important;
    justify-content: center !important;
    -webkit-box-align: center !important;
    -ms-flex-align: center !important;
    align-items: center !important;
  }
  .__form .__email .__Forename,
  .__form .__message .__Forename {
    width: 290px !important;
  }
  #__info {
    -webkit-box-align: start !important;
    -ms-flex-align: start !important;
    align-items: flex-start !important;
    width: max-content !important;
    margin-top: 2rem;
  }
  #__info .__Itext {
    font-size: 18px !important;
  }
  #__info ._Mul,
  #__info .__Itext {
    text-align: left !important;
    font-size: 13px !important;
  }
  .__chart {
    width: 200px !important;
  }
  .__chart label {
    font-size: 9px !important;
  }
  .__loc {
    padding: 0.3rem 0.6rem !important;
  }
  .__loc .__bolder {
    font-size: 13px !important;
  }
  .__loc .__address {
    font-size: 12px !important;
  }
  .__HomeScreen .__contact .__contactContainer .__form .__conditions {
    align-items: center;
  }
  .__HomeScreen .__contact .__contactContainer .__form .__conditions button {
    margin: 3rem 0 0 0;
    background-color: #00a343;
    color: white;
    padding: 1rem 6rem;
    border: none;
    cursor: pointer;
  }
}
/*# sourceMappingURL=style.css.map */
</style>
