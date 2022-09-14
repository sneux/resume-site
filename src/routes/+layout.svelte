<header>
    <img class="logo" src="https://i.ibb.co/TLBxnbw/jhgjghjgj.png" style="width: 78px; height: 57px;" />

    <nav>
        <ul class="nav_links">
            <li><a href="#">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>

        </ul>
    </nav>

</header>

<style>
    header {
    height: 35px;
    max-width: 100vw;
    position: fixed;
    top: 0;
    z-index: 1000;
    left: 0;
    right: 0;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
    color: rgb(150, 198, 245);
    padding: 30px 10%;
    line-height: 20px;

}

/* header logo */
/* Style the logo link (notice that we set the same value of line-height and font-size to prevent the header to increase when the font gets bigger */
.logo {
    left: 0;
  }
  
.nav_links {
  list-style: none;
}

.nav_links li {
  display: inline-block;
  padding: 0px 20px;
}

.nav_links li a {
  transition: all 0.3s ease 0s;
}

.nav_links li a:hover {
  color: black;
}

  /* Change the background color on mouse-over */
  .header a:hover {
    background-color: rgb(225, 244, 255);
    color: black;
  }
  
  /* Style the active/current link*/
  .header a.active {
    background-color: rgb(150, 198, 245);
    color: white;
  }
  
  /* Float the link section to the right */
  .header-right {
    margin-top: 0%;
    text-align: right;
  }
  
  /* Add media queries for r
  position: absolute;esponsiveness - when the screen is 500px wide or less, stack the links on top of each other */
  @media screen and (max-width: 1000px) {
    .header a {
      float: none;
      display: block;
      text-align: left;
    }
    .header-right {
      float: none;
    }
  }

/* SCROLL BAR */
/* width */
::-webkit-scrollbar {
  width: 7px;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 5px rgb(173, 173, 173);
  border-radius: 10px;
}

</style>
<slot>

</slot>