
<!--Drawer-->
<div class="drawer">
    <input id="my-drawer-3" type="checkbox" class="drawer-toggle" /> 
    <div class="drawer-content flex flex-col">
      <!-- Navbar -->
      <div class="w-full navbar bg-base-100">
        <div class="flex-1 mx-auto">
          <a href="/" class="btn btn-ghost normal-case text-xl"><img src="ftbLogo.png"></a>
        </div>
        <div class="flex-1">
          <a class="btn btn-ghost normal-case text-xl"><img src="ftbText.png"></a>
        </div>
        <div class="flex-none hidden lg:block">
          <ul class="menu menu-horizontal">
            <!-- Navbar menu content here -->
            <li><a href="/about">About</a></li>
            <li><a href="/staff">Teachers & Philosophy</a></li>
            <li><a>Services</a></li>
            <li><a>Infants</a></li>
            <li><a>Toddlers</a></li>
            <li><a>Preschool</a></li>
            <li><a>Beginners</a></li>
            <li><a>Pre-K</a></li>
            <li><a>After-School</a></li>
            <li><a>Contact</a></li>     
          </ul>
        </div>
        <div class="flex-none lg:hidden">
          <label for="my-drawer-3" class="btn btn-square btn-ghost">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-6 h-6 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
          </label>
      </div> 
  </div>

<slot />

  <footer class="footer footer-center p-10 bg-base-200 text-base-content rounded">
      <div class="grid grid-flow-col gap-4">
        <a class="link link-hover">About us</a> 
        <a class="link link-hover">Contact</a> 
        <a class="link link-hover">Careers</a> 
        <a class="link link-hover">Services</a>
        <a class="link link-hover">Feedback</a>
      </div>
      <div>
        <div class="grid grid-flow-col gap-4">
          <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"></path></svg></a> 
          <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"></path></svg></a> 
          <a><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" class="fill-current"><path d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"></path></svg></a>
        </div>
      </div>
      <div>
        <h1>Hours of Operation:</h1>
          <p>Mon-Fri	6:30 AM - 6:00 PM</p>
          <p> Sat-Sun	Closed</p>
        <p>Copyright © 2023 - All right reserved by ACME Industries Ltd</p>
      </div>
  </footer>

</div>
<!-- End Drawer-->
<!--Drawer Side Menu-->
    <div class="drawer-side">
      <label for="my-drawer-3" class="drawer-overlay"></label> 
        <ul class="menu p-4 w-80 bg-base-100">
            <!-- Sidebar content here -->
            <li><a href="/about">About Us</a></li>
            <li><a href="/staff">Teachers & Philosophy</a></li>
            <!-- Collapsible-->
            <div class="collapse collapse-arrow">
                <input type="checkbox" /> 
                <div class="collapse-title">
                  <li><a href="/childcare">Childcare</a><li>
                </div>
                <div class="collapse-content"> 
                  <li><a>Infants</a></li>
                  <li><a>Toddlers</a></li>
                  <li><a>Preschool</a></li>
                  <li><a>Beginners</a></li>
                  <li><a>Pre-K</a></li>
                  <li><a>After-School</a></li>
                </div>
            </div>
            <li><a href="/feedback">Family Feedback</a></li> 
            <li><a href="/contact">Contact Us</a></li>
        </ul>
    </div>
    
  </div>



   <div class="btm-nav">
    <a href="/email">
    <button class="text-error"> 
            <svg xmlns="http://www.w3.org/2000/svg" class="h-7.5 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
            <span style="" class="btm-nav-label">Email</span>  
    </button>
  </a> 
    <a href="/phone">
      <button class="text-success">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-7.5 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
      <span style="" class="btm-nav-label">Phone</span>
    </button>
    </a>
    <a href="/location">
    <button class="text-warning">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-7.5 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path d="M12 22s-8-4.5-8-11.8A8 8 0 0 1 12 2a8 8 0 0 1 8 8.2c0 7.3-8 11.8-8 11.8z"/><circle cx="12" cy="10" r="3"/></svg>
      <span style="" class="btm-nav-label">Location</span>
    </button>
    </a>
    <a href="/messenger">
    <button class="text-info">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-7.5 w-10" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
        <span style="" class="btm-nav-label">Facebook</span>
    </button>
    </a>
    <div class="flex-none lg:hidden">
      <label for="my-drawer-3" class="btn btn-square btn-ghost">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-6 h-6 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
      </label>
    </div>  
  </div>









