document.getElementById('addBtn').addEventListener('click', function() {
  const taskInput = document.getElementById('taskInput');
  const taskText = taskInput.value.trim();

  if (taskText !== '') {
    const li = document.createElement('li');

    const checkbox = document.createElement('input');
    checkbox.type = 'checkbox';

    const taskSpan = document.createElement('span');
    taskSpan.textContent = taskText;

    checkbox.addEventListener('change', function() {
      li.classList.toggle('done');
    });

    taskSpan.addEventListener('click', function() {
      li.classList.toggle('done');
      checkbox.checked = li.classList.contains('done');
    });

    li.appendChild(checkbox);
    li.appendChild(taskSpan);

    document.getElementById('taskList').appendChild(li);
    taskInput.value = '';
  }
});
