<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="container">
    <h1>Delete Account</h1>
    <p>Please select a reason for deleting your account:</p>
    <form id="delete-form">
      <div class="form-group">
        <label for="reason">Reason:</label>
        <select id="reason" required>
          <option value="">Select a reason</option>
          <option value="no-longer-needed">No longer needed</option>
          <option value="privacy-concerns">Privacy concerns</option>
          <option value="unsatisfied-service">
            Unsatisfied with the service
          </option>
          <option value="moving-platforms">Moving to another platform</option>
          <option value="other">Other</option>
        </select>
      </div>
      <button type="submit">Delete Account</button>
    </form>
  </div>
</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 20px;
}

h1 {
  color: #333;
  font-size: 24px;
}

.container {
  max-width: 400px;
  margin: 0 auto;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

select {
  width: 100%;
  padding: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  padding: 10px 20px;
  font-size: 16px;
  background-color: #333;
  color: #fff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #555;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
