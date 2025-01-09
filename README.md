<style>
        @import url('https://fonts.googleapis.com/css2?family=Koulen&display=swap');

        *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: 16px;
        }

        :root{
            --fs-apresentation-super-title: 2rem;
            --fs-header-title: 2rem;
            --fs-header-subtitle: 18px;
            --margin-header: 0;
            --margin-gap: 0;
        }
        
        @media (min-width: 1024px){
            :root{
                --fs-apresentation-super-title: 4rem;
                --margin-header: 10rem;
                --margin-gap: 10rem;
            }
        }
    
        header{
            position: relative;
            color:white;

            img{
                width: 100%;
            }

            &>.header-container{
                position: absolute;
                width: 100%;
                height: 100%;
                top: 0;
                left: 0;


                &>.principal-apresentation{
                    width: 100%;
                    text-align: center;
                    margin-block: var(--margin-header);
                    font-size: var(--fs-apresentation-super-title);
                    font-family: "Koulen", serif;
                    font-weight: 400;
                }

                &>.apresentations{

                    & .first-apresentation, & .second-apresentation{
                        & h1{
                            font-size: var(--fs-header-title);
                            font-weight: 700;
                            margin-bottom: .5rem;
                        }

                        &:has(p:nth-of-type(2)) p:nth-child(2){
                            font-size: var(--fs-header-subtitle);
                            font-weight: 600;
                        }
                    }

                    & .first-apresentation{
                        width: 500px;
                        margin-bottom: var(--margin-gap);
                    }

                    & .second-apresentation{
                        text-align: right;
                    }
                }
            }
        }
    </style>
    
<header>
    <img src="./images/background_principal.png">
    <div class="header-container">
        <h1 class="principal-apresentation">OPA ✌, TUDO BEM?</h1>
        <section class="apresentations">
            <section class="first-apresentation">
                <h1>Vinícius Borges</h1>
                <p>Programador Fullstack & Designer UX/UI</p>
                <p>Carinhosamente apelidado de “O Dev que Tudo Vê”, faço
                    da programação uma arte. Acredito que cada linha de
                    código deve ser vista e contemplada por todos.</p>
            </section>
            <section class="second-apresentation">
                <h1>O dev que tudo vê</h1>
                <p>Eu consigo te ver, então mantenha seus olhos em
                    <em>mim</em></p>
            </section>
        </section>
    </div>
</header>