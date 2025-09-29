// script.js - Interactive Features

// Progress tracking (uses localStorage for persistence)
// Note: If deploying to Claude.ai, replace with in-memory storage

let progress = {
    currentDay: 0,
    completedTasks: [],
    weeklyProgress: { week1: 0, week2: 0, week3: 0 }
};

// Load progress from localStorage (or initialize)
function loadProgress() {
    const saved = localStorage.getItem('bootcampProgress');
    if (saved) {
        progress = JSON.parse(saved);
    }
    updateProgressDisplay();
}

// Save progress
function saveProgress() {
    localStorage.setItem('bootcampProgress', JSON.stringify(progress));
}

// Update visual progress indicators
function updateProgressDisplay() {
    const progressBar = document.querySelector('.progress-fill');
    const percentage = (progress.currentDay / 21) * 100;
    progressBar.style.width = percentage + '%';
    progressBar.textContent = `Day ${progress.currentDay} of 21`;
    
    // Update week cards
    updateWeekCards();
}

// Task checkbox handling
document.addEventListener('DOMContentLoaded', function() {
    const checkboxes = document.querySelectorAll('.task-list input[type="checkbox"]');
    
    checkboxes.forEach((checkbox, index) => {
        // Load saved state
        if (progress.completedTasks.includes(index)) {
            checkbox.checked = true;
        }
        
        // Save on change
        checkbox.addEventListener('change', function() {
            if (this.checked) {
                if (!progress.completedTasks.includes(index)) {
                    progress.completedTasks.push(index);
                }
            } else {
                progress.completedTasks = progress.completedTasks.filter(t => t !== index);
            }
            saveProgress();
            checkDayCompletion();
        });
    });
    
    loadProgress();
});

// Check if day is complete
function checkDayCompletion() {
    const totalTasks = document.querySelectorAll('.task-list input[type="checkbox"]').length;
    const completedCount = progress.completedTasks.length;
    
    if (completedCount === totalTasks && totalTasks > 0) {
        showCompletionMessage();
        progress.currentDay++;
        saveProgress();
        updateProgressDisplay();
    }
}

// Show motivational message
function showCompletionMessage() {
    const messages = [
        "Excellent work! You're building real skills! 🎉",
        "Day completed! You're one step closer to your goal! 💪",
        "Keep going! Consistency is key! 🌟",
        "Great progress! You're becoming a financial analyst! 📊"
    ];
    
    const randomMessage = messages[Math.floor(Math.random() * messages.length)];
    alert(randomMessage);
}

// Update week card statuses
function updateWeekCards() {
    const cards = document.querySelectorAll('.week-cards .card');
    
    cards.forEach((card, index) => {
        const statusSpan = card.querySelector('.status');
        const weekNum = index + 1;
        const startDay = (weekNum - 1) * 7;
        const endDay = weekNum * 7;
        
        if (progress.currentDay >= endDay) {
            statusSpan.textContent = 'Completed';
            statusSpan.className = 'status completed';
        } else if (progress.currentDay >= startDay) {
            statusSpan.textContent = 'In Progress';
            statusSpan.className = 'status in-progress';
        } else if (progress.currentDay >= startDay - 7 || weekNum === 1) {
            statusSpan.textContent = 'Not Started';
            statusSpan.className = 'status not-started';
        } else {
            statusSpan.textContent = 'Locked';
            statusSpan.className = 'status locked';
        }
    });
}