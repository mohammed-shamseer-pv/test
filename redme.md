@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,300;0,400;0,500;1,100;1,200;1,300;1,400;1,500&display=swap');

:root{
  --color:#069f1f;
}

*{
  font-family: 'Poppins', sans-serif;
  margin:0; padding:0;
  box-sizing: border-box;
  text-transform: capitalize;
  transition: all .2s linear;
  text-decoration: none;
}

html{
  font-size: 62.5%;
}

body{
  overflow-x: hidden;
}

.heading{
    margin:2rem;
    padding-top: 6rem;
    display: inline-block;
    font-size: 3.5rem;
    color:var(--color);
    position: relative;
    letter-spacing: .2rem;
  }
  
  .heading::before, .heading::after{
    content: '';
    position: absolute;
    height: 2.5rem;
    width: 2.5rem;
    border-top:.4rem solid var(--color);
    border-left:.4rem solid var(--color);
  }
  
  .heading::before{
    top:5.8rem; left: -2rem;
  }
  
  .heading::after{
    bottom:-.5rem; right: -2rem;
    transform: rotate(180deg);
  }
  

.btn{
  outline: none;
  border: none;
  border-radius: 5rem;
  background: var(--color);
  color:#fff;
  cursor: pointer;
  height:3.5rem;
  width: 15rem;
  font-size: 1.7rem;
  box-shadow: 0 .2rem .5rem rgba(0,0,0,.3);
}

.btn:hover{
  letter-spacing: .1rem;
  opacity: .8;
}













.header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  padding:1rem 2rem;
  position: fixed;
  top:0; left: 0;
  z-index: 100;
 
}

.header .logo{
  font-size: 2.5rem;
  color:#fff;
}

.header .logo i{
  padding:0 .5rem;
}

.header .navbar ul{
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.header .navbar ul li{
  margin:0 1.5rem;
}

.header .navbar ul li a{
  font-size: 2rem;
  color:#fff;
}

.header .navbar ul li a:hover{
  color:#ccc;
}

.header .fa-bars{
  color:#fff;
  cursor: pointer;
  font-size: 3rem;
  display: none;
}
.logo1{
    width: auto;
    height: 60px;
}






.home{
  min-height: 100vh;
  width: 100vw;
  background:linear-gradient(rgb(120, 227, 129), var(--color));
  display: flex;
  align-items: center;
  justify-content: center;
  flex-flow: column;
  text-align: center;
  padding:0 1rem;
  position: relative;
  overflow: hidden !important;
}

.home .banner{
  color:#fff;
  font-size: 5rem;
  text-shadow: 0 .3rem .5rem rgba(0,0,0,.3);
}

.home .slogan{
  color:#eee;
  font-size: 2.5rem;
  font-weight: 400;
}

.home button{
  height: 6rem;
  width: 19rem;
  background:#fff;
  color: #444;
  cursor: pointer;
  border:none;
  border-radius: 111px;
  outline: none;
  margin-top: 1rem;
  font-size: 2rem;
  font-weight: 400;
  box-shadow: 0 .3rem .5rem rgba(0,0,0,.3);
}

.home button:hover{
  letter-spacing: .1rem;
}

.home .wave{
  position: absolute;
  bottom: -.5rem;
  left: 0;
  height:11rem;
  width: 100%;
  background: url(../images/wave.png);
  background-size: 100rem 11rem;
  background-repeat: repeat-x;
  animation:waves 10s linear infinite;
}

.home .wave2{
  animation-direction: reverse;
  opacity: .2;
}

.home .wave3{
  animation-duration: 4s;
  opacity: .5;
}

@keyframes waves{
  0%{
    background-position-x: 0;
  }
  100%{
    background-position-x: 100rem;
  }
}

.home .fa-cog{
  position: absolute;
  font-size: 30rem;
  opacity: .15;
  color:#fff;
  animation: rotate 10s linear infinite;
}

.home .nut1{
  top:10%; left: -15rem;
}

.home .nut2{
  bottom:23%; right: -13rem;
  animation-direction: reverse;
}

@keyframes rotate{
  100%{
    transform: rotate(360deg);
  }
}



.service{
    width: 100vw;
    text-align: center;
    margin-top: 9rem;
  }
  
  .service .row{
    margin:2rem 0;
    padding:0 2rem;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  
  .service .row .image img{
    width:50vw;
    height:55vh;
  }
  
  .service .row .content{
    text-align: left;
    padding:0 3rem;
  }
  
  .service .row .content h3{
    font-size: 3rem;
    color:var(--color);
  }
  
  .service .row .content p{
    font-size: 1.5rem;
    color:#333;
    padding:1rem 0;
  }
  




  
.faq{
    min-height: 100vh;
    width: 100vw;
    text-align: center;
    padding:0 2rem;
  }
  
  .faq .row{
    display: flex;
    align-items: center;
    justify-content: center;
    padding:0 2rem;
  }
  
  .faq .row .image img{
    height:70vh;
    width:50vw;
  }
  
  .faq .row .accordion-container{
    width: 50%;
    text-align: left;
  }
  
  .faq .row .accordion-container .accordion .accordion-header{
    background-color: var(--color);
    margin:1rem 0;
    box-shadow: .1rem .1rem .3rem rgba(0,0,0,.3);
    cursor: pointer;
  }
  
  .faq .row .accordion-container .accordion .accordion-header span{
    display: inline-block;
    text-align: center;
    height:4rem;
    width:5rem;
    line-height: 4rem;
    font-size: 2rem;
    background:#fff;
    color:#333;
    clip-path: polygon(0% 0%, 75% 0%, 100% 50%, 75% 100%, 0% 100%);
  }
  
  .faq .row .accordion-container .accordion .accordion-header h3{
    display: inline;
    color: #fff;
    font-weight: 400;
    padding-left: .5rem;
    font-size: 1.5rem;
  }
  
  .faq .row .accordion-container .accordion .accordion-body{
    padding:1rem;
    color:#444;
    box-shadow: .1rem .1rem .3rem rgba(0,0,0,.3);
    font-size: 1.3rem;
    display: none;
  }
  
  .faq .row .accordion-container .accordion:nth-child(1) .accordion-body{
    display: block;
  }
  

/* 
Responseev */




/* media queries  */

@media (max-width:768px){

    html{
      font-size: 50%;
    }
  
    .header .fa-bars{
      display: block;
    }
  
    .header .navbar{
      position: fixed;
      top:-120%; left: 0;
      height: auto;
      width: 100%;
      background-color: #fff;
      z-index: 1000;
      border-top: .1rem solid rgba(0,0,0,.3);
    }
  
    .header .navbar ul{
      height: 100%;
      width: 100%;
      flex-flow: column;
    }
  
    .header .navbar ul li{
      margin:1rem 0;
    }
  
    .header .navbar ul li a{
      color: #444;
      font-size: 2.4rem;
    }
  
    .header .fa-times{
      transform: rotate(180deg);
    }
  
    .header .nav-toggle{
      top:5.8rem;
    }
  
    .home .banner{
      font-size: 4rem;
    }
  
    .home .slogan{
      font-size: 1.7rem;
    }
  
    .about .row{
      flex-flow: column-reverse;
      padding:0 2rem;
    }
  
    .about .row .image img{
      width: 100vw;
    }
  
    .service .row{
      flex-flow: column-reverse;
    }
  
    .service .row:nth-child(even){
      flex-flow: column;
    }
  
    .service .row .image img{
      width: 100vw;
    }
  
    .service .row .content{
      padding:0;
    }
  
    .contact .row{
      flex-flow: column;
    }
  
    .contact .row .image img{
      width: 100vw;
    }
  
    .contact .row .form-container{
      width: 100%;
      padding:0 1.5rem;
    }
  
    .faq{
      padding:0;
    }
  
    .faq .row{
      padding:0 1rem;
      flex-flow: column;
    }
  
    .faq .row .image img{
      width:100vw;
    }
  
    .faq .row .accordion-container{
      width:100%;
    }
  
  }
  
  @media (max-width:550px){
    .footer{
      flex-flow: column;
    }
    .footer h1{
      text-align: center;
    }
    .footer .icons{
      padding:2rem 0;
    }
  }




      background-image: url(https://cdn.pixabay.com/photo/2020/04/12/18/13/background-5035258_960_720.jpg);
    background-size: cover;

    