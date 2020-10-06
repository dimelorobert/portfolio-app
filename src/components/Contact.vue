<template>
  <div class="container">
    <div class="container__contact">
      <div class="contact__banner">
        <div class="contact__banner--info">
          <h2>
            Contacto
          </h2>
            <p>
              “You've seen the goods, now meet the man.
              Reach out and let us consider joining forces for the greater good.”
            </p>
        </div>
          <div class="contact__banner--social">
            <div class="social__horizontal">
              <div class="social__horizontal--all">
                <div id="contact" class="social__horizontal--column">
                  <div>
                    <img src="@/assets/Github2.png" alt="github">
                    <h2>
                    Github
                  </h2>
                  </div>
                  <p>
                    Proyectos, ejercicios, y READMEs... <br>
                    <a class="social" href="https://github.com/JuanLoyola" target="_blank">Ver perfil</a>
                  </p>
                </div>
              </div>
              <div>
                <div class="social__horizontal--all">
                <div class="social__horizontal--column">
                  <div>
                    <img src="@/assets/linkedin2.png" alt="linkedin">
                    <h2>
                      LinkedIn
                    </h2>
                  </div>
                  <p>
                    Ya conoces el procedimiento. <br>
                    <a class="social" href="https://www.linkedin.com/in/LoyolaJuan" target="_blank">Ver perfil</a>
                  </p>
                </div>
              </div>
              </div>
              <div>
                <div class="social__horizontal--all">
              <div class="social__horizontal--column">
                <div>
                  <img class="email" src="@/assets/email.png" alt="email">
                  <h2>
                    Email
                  </h2>
                </div>
                <p>
                  ¿Quien no tiene uno?
                </p>
                <a href="mailto:juan.loyola1@hotmail.com" class="social">
                  Enviar email
                </a>
              </div>
                </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  .container{
    width: 100%;
    height: 100%;
    margin-bottom: 50px;
    display:flex;
    &__contact{
      width: 100%;
      display:flex;
      justify-content: center;
      align-items: center;
      .contact__banner{
        background: linear-gradient(90deg, #ECE9E6 0%, #FFFFFF 100%);
        box-shadow: 0px 4px 11px rgba(0, 0, 0, 0.5);
        border-radius: 9px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
        height: 70vh;
      }
      .contact__banner--info{
        display:flex;
        justify-content: center;
        align-items: center;
        flex-direction:column;
        padding: 2rem 5rem;
      }
      .contact__banner--info h2{
        font-family: 'Poppins';
        font-size: 48px;
        line-height: 72px;
        display:flex;
        justify-content: flex-start;
        align-items: flex-start;

        color: #333333;
        text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.36);
      }
      .contact__banner--info p{
        font-family: 'Poppins';
        font-size: 15px;
        line-height: 22px;
        margin-top: 30px;
        display: flex;
        align-items: center;
        text-align: center;

        color: #000;
      }
      .contact__banner--social{
        display:flex;
        justify-content: space-evenly;
        align-items: center;
        width: 100%;
        .social__horizontal{
          display:flex;
          align-items: center;
          justify-content: space-around;
          width: 100%;
          .social__horizontal--all img{
            width: 70px;
            margin: 10px;
            filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
          }
          .social__horizontal--all{
            display:flex;
            flex-direction: row;
            align-items: center;
          }
          .social__horizontal--column{
            display:flex;
            flex-direction: column;

            font-family: 'Poppins';
            font-size: 15px;
            line-height: 40px;

            color: #000000;

            .email{
              height: 70px;
              width: auto;
              filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
            }
          }
          .social{
            text-decoration: none;
            display:flex;
            justify-content: center;
            align-content: flex-end;
            border: 1px solid #7389E1;
            border-radius: 5px;
            padding: 5px 5px;
          }
          .social:hover{
            background-color:#7389E1;
            color: #fff;
            transition: linear 500ms;
            cursor: pointer;
          }
        }
      }
    }
  }
</style>

<script>
export default {
  name: 'Contact'
}
</script>
