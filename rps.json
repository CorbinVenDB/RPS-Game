const compChoice = getComputerChoice();
const humanChoice = getHumanChoice();
let outcome = playRound();
let humanScore = 0
let computerScore = 0

function getComputerChoice() {
    let number = (Math.floor(Math.random() * 3) + 1);
    if (number === 1) {
    return "rock";
    }
    else if (number === 2) {
        return "paper";
    }
    else if (number === 3) {
        return "scissors";
    }
}

function getHumanChoice () {
    let input = prompt("Rock, Paper, Scissors! Choose your weapon!");
    return input.toLocaleLowerCase();
}

function playRound () {
    if (humanChoice === compChoice) {
        return "Tie"
    }
    else if (humanChoice === "rock" && compChoice === "scissors") {
        return "Rock beats Scissors! You Win!";
        humanScore++;
    }
    else if (humanChoice === "rock" && compChoice === "paper") {
        return "Paper beats Rock! You Loose!";
    }
    else if (humanChoice === "paper" && compChoice === "scissors") {
        return "Scissors beats Paper! You Loose!";
    }
    else if (humanChoice === "paper" && compChoice === "rock") {
        return "Paper beats Rock! You Win!";
    }
    else if (humanChoice === "scissors" && compChoice === "paper") {
        return "Scissors beats Paper! You Win!";
    }
    else if (humanChoice === "scissors" && compChoice === "rock") {
        return "Rock beats scissors! You Loose!";
    }
}

playRound(humanChoice, compChoice);

console.log("Human Choice: ", humanChoice);
console.log("Computer Choice: ", compChoice);
console.log(outcome);
console.log("Wins: ", humanScore);
console.log("Losses: ", computerScore);
