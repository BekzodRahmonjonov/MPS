<template>
  <div class="container">
    <div class="company features">
      <div class="company__creative-marketing">
        <h5 class="pink-heading">Features</h5>
        <h2 class="company__heading">Smart Complex Solutions</h2>
        <p class="paragraph">
          Stars had ceased to twinkle the same illusion which lifts the horizon
          of the sea to the level of the spectator on a hillside, the sable
          cloud beneath was dished out.
        </p>
        <div class="card">
          <h4 class="heading_sm">
            <svg
              width="24"
              height="23"
              viewBox="0 0 24 23"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M8.332 7.62569L12 0L15.668 7.6267L24 8.78546L17.936 14.6569L19.416 22.999L12 19.0028L4.584 23L6.064 14.6579L0 8.78546L8.332 7.62569ZM14.335 9.47468L12 4.62096L9.665 9.47468L4.36 10.2133L8.221 13.9515L7.279 19.2617L12 16.7175L16.721 19.2607L15.779 13.9505L19.64 10.2123L14.335 9.47468Z"
                fill="#4DB282"
              />
            </svg>
            <span>Modern Technology</span>
          </h4>
          <p class="paragraph">
            The sky was cloudless and of a deep dark blue the spectacle before
            us was indeed sublime.
          </p>
        </div>
      </div>
      <div class="company__img">
        <img class="company__img-item" src="../assets/features-img.png" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.features {
  .company__heading {
    font-size: 56px;
  }
  .card {
    padding: 28px 32px;
    background: #ffffff;
    box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
    border-radius: 8px;
    margin-top: 20px;
    .heading_sm {
      font-family: "Hind Siliguri";
      font-style: normal;
      font-weight: bold;
      font-size: 24px;
      line-height: 32px;
      color: #333333;
      display: flex;
      gap: 10px;
    }
    .paragraph {
      font-family: "Work Sans";
      font-style: normal;
      font-weight: normal;
      font-size: 14px;
      line-height: 24px;
      color: rgba(51, 51, 51, 0.496405);
      margin-top: 6px;
    }
  }
}
</style>
