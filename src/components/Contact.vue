<template>
  <div class="container">
    <div class="container__contact">
      <div class="contact__banner">
        <div class="contact__banner--info">
          <h2>
            {{$t('contact.title')}}
          </h2>
            <p>
              {{$t('contact.sentence')}}
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
                    <a class="social" href="https://github.com/JuanLoyola" target="_blank">{{$t('contact.btn')}}</a>
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
                    <a class="social" href="https://www.linkedin.com/in/LoyolaJuan" target="_blank">{{$t('contact.btn')}}</a>
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
                <a href="mailto:juan.loyola1@hotmail.com" class="social">
                  {{$t('contact.email')}}
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
        background-image: url('../assets/contact.svg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: 700px;
        box-shadow: 0px 4px 11px rgba(0, 0, 0, 0.5);
        border-radius: 9px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
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
        font-size: 2em;
        color: #fff;
        font-weight: bold;
        line-height: 72px;
        display:flex;
        justify-content: flex-start;
        align-items: flex-start;
        text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.36);
      }
      .contact__banner--info p{
        font-family: 'Poppins';
        font-size: 1rem;
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
            background-color:#7389E1;
            color: #fff;
            border-radius: 5px;
            padding: 5px 5px;
          }
          .social:hover{
            background-color:#9babeb;
            color: #f1f1f1;
            transition: linear 500ms;
            cursor: pointer;
          }
        }
      }
    }
  }

  @media screen and (min-width:320px) and (max-width: 1024px) {
    .container{
    &__contact{
      width: 100%;
      .contact__banner{
        width: 90%;
        background-size: 70%;
        box-shadow: 0px 4px 11px rgba(0, 0, 0, 0.5);
        border-radius: 9px;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
      }
      .contact__banner--social{
        .social__horizontal{
          .social__horizontal--all img{
            width: 30px;
            margin: 5px;
            filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
          }
          .social__horizontal--all{
            display:flex;
            flex-direction: row;
            align-items: center;
          }
          .social__horizontal--column{
            display:flex;
            flex-flow: column;

            font-family: 'Poppins';
            font-size: 0.5rem;
            line-height: 20px;

            color: #000000;

            .email{
              height: 30px;
              filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
            }
          }
          .social{
            text-decoration: none;
            border: 1px solid #7389E1;
            border-radius: 2px;
            padding: 0px 5px;
            font-size: 0.5rem;
            display:flex;
            justify-content: center;
            align-items: center;
            margin: 2px;
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
    }

  @media screen and (min-width:320px) and (max-width: 320px){
  }
</style>

<script>
export default {
  name: 'Contact'
}
</script>
