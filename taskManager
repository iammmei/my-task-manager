const readline = require("readline");
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

function taskManagerDisplay() {
  console.log("Welcome to your task manager. Press:");
  console.log("1. to see all your tasks");
  console.log("2. to add a task");
  console.log("3. to delete a task");
  console.log("4. to mark a task as done");
  console.log("5. to Exit the task manager");
}

function SelectChoice(choice) {
  switch (choice) {
    case "1":
      console.log("You selected option 1: See all tasks");

      break;
    case "2":
      console.log("You selected option 2: Add a task");

      break;
    case "3":
      console.log("You selected option 3: Delete a task");

      break;
    case "4":
      console.log("You selected option 4: Mark a task as done");

      break;
    case "5":
      console.log("Exiting the task manager. Goodbye!");
      rl.close();
      break;
    default:
      console.log("Invalid choice. Please select a valid option.");
      break;
  }
}

function printMenuChoice() {
  rl.question("Enter your choice: ", (choice) => {
    SelectChoice(choice);
    if (choice !== "5") {
      taskManagerDisplay();
      printMenuChoice();
    }
  });
}

taskManagerDisplay();
printMenuChoice();
