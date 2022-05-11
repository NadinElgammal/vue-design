<template>
  <section>
    <div class="content">
      <div class="search-part">
        <div class="searchBar">
          <input id="searchQueryInput" type="text" name="searchQueryInput" value="" />
          <button id="searchQuerySubmit" type="submit" name="searchQuerySubmit">
          <i class="fa-solid fa-magnifying-glass search-icon"></i>
          </button>
        </div>
        <div class="save-icon">
          <i class="fa-solid fa-bookmark saved-icon "></i>
        </div>
        <div class="icon">
          <i class="fa-solid fa-arrow-up-wide-short filter-icon"></i>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Products",
};
</script>

<style scoped>
.search-part {
  padding: 20px 20px;
  display: flex;
  gap: 20px;
  justify-content: flex-end;
}
.icon {
  background-color: #0E0E0F;
  border-radius: 50px;
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.save-icon {
  background-color: #9d5cff;
  border-radius: 50px;
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.filter-icon,
.saved-icon {
  color: white;
}


.wrapper {
  width: 100%;
  max-width: 31.25rem;
  margin: 6rem auto;
}

.label {
  font-size: .625rem;
  font-weight: 400;
  text-transform: uppercase;
  letter-spacing: +1.3px;
  margin-bottom: 1rem;
}

.searchBar {
  width: 250px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

#searchQueryInput {
  width: 100%;
  height: 2.8rem;
  background: #ffffff;
  outline: none;
  border: none;
  border-radius: 1.625rem;
  padding: 0 0 0 1.5rem;
  font-size: 1rem;
}

#searchQuerySubmit {
  width: 3.5rem;
  height: 2.8rem;
  margin-left: -3.5rem;
  background: none;
  border: none;
  outline: none;
  color: #848791;
}

#searchQuerySubmit:hover {
  cursor: pointer;
}
</style>