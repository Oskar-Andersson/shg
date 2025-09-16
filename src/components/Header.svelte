<script>
  export let title = '';
  const base = ''; // subdomain root
</script>

<div class="row d-flex header" style="z-index: 1; min-height: 140px; background-color:rgba(0, 0, 0, 0.6);">
  <div class="col-md-1"></div>
  <div class="col-md-10" style="flex: 1 1 auto; opacity: 1;">
    <div class="row d-flex pb-2 h-100">
      <div class="col-md-4 align-self-end">
        <div class="row mb-2 d-flex text-start justify-content-start" style="width: 160px;">
          <div class="col-md-auto align-self-end">
            <a href="https://open.spotify.com/artist/6W8a9qf3p13KUAR5pDLpEM?si=39d9f0065a254e3b">
              <img alt="Spotify icon" src={"/spotify.svg"} style="height: 35px;">
            </a>
          </div>
          <div class="col-md-auto align-self-end">
            <a href="https://www.facebook.com/profile.php?id=100003203298990">
              <img alt="Facebook icon" src={"/facebook.svg"} style="height: 35px;">
            </a>
          </div>
        </div>
      </div>

      <div class="col-md-4 ">
        <div class="row justify-content-center">
          <div class="col-md-auto" style="color: #D3A786; font-family: 'PT Sans', sans-serif; font-size: 4em; font-weight:500;">
            {title}
          </div>
        </div>
      </div>

      <div class="col-md-4 d-flex flex-row justify-content-between align-self-end">
        <div style="padding: 6px;"><a style="display: inline-block; color: #DEB79A; text-decoration: none; font-size: 1.2em;" href={base + "/"}>Home</a></div>
        <div style="padding: 6px;"><a style="display: inline-block; color: #DEB79A; text-decoration: none; font-size: 1.2em;" href={base + "/bio"}>Biography</a></div>
        <div style="padding: 6px;"><a style="display: inline-block; color: #DEB79A; text-decoration: none; font-size: 1.2em;" href={base + "/music"}>Music</a></div>
        <div style="padding: 6px;"><a style="display: inline-block; color: #DEB79A; text-decoration: none; font-size: 1.2em;" href={base + "/gallery"}>Gallery</a></div>
        <div style="padding: 6px;"><a style="display: inline-block; color: #DEB79A; text-decoration: none; font-size: 1.2em;" href={base + "/contact"}>Contact</a></div>
      </div>
    </div>
  </div>
  <div class="col-md-1"></div>
</div>

<style>
.header {
  font-family: 'Karla', sans-serif;
}
</style>
