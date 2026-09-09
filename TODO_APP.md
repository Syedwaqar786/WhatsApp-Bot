# To-Do List Application

A complete To-Do List application with local storage functionality using JSON.

## Features

✅ **Core Functionality:**
- ➕ Add new todos with title, description, and priority
- 📝 View all todos in formatted display
- ✅ Mark todos as completed/incomplete
- 🗑️ Delete todos
- ✏️ Update existing todos
- 📊 View statistics about tasks

✅ **Local Storage:**
- 💾 Automatic JSON file storage
- 📂 Persistent data between sessions
- 🔒 Safe file handling

✅ **Filtering & Organization:**
- 🔍 Filter by status (all, completed, pending)
- 🎯 Filter by priority (high, medium, low)
- 📈 Completion rate tracking

✅ **User Interface:**
- 🎯 Interactive CLI menu
- 📋 Formatted todo display
- 🌍 Urdu language support
- 😊 Emoji indicators for visual clarity

## Installation

```bash
pip install -r requirements.txt
```

## Usage

### Run the Application

```bash
python todo_app.py
```

### Programmatic Usage

```python
from todo_app import TodoListApp

# Initialize app
app = TodoListApp("my_todos.json")

# Add a todo
app.add_todo("پروجیکٹ مکمل کریں", "GitHub پروجیکٹ تیار کریں", "high")

# View todos
app.display_todos()

# Mark as completed
app.mark_completed(1)

# Get statistics
app.display_statistics()
```

## Commands

| Command | Description |
|---------|-------------|
| `add` | نیا کام شامل کریں |
| `list` | تمام کام دیکھیں |
| `complete` | کام مکمل کریں |
| `delete` | کام حذف کریں |
| `update` | کام اپڈیٹ کریں |
| `stats` | اعدادوشمار دیکھیں |
| `filter` | فلٹر کریں |
| `exit` | باہر نکلیں |

## Storage Format

Todos are stored in `todos.json`:

```json
[
  {
    "id": 1,
    "title": "پروجیکٹ مکمل کریں",
    "description": "GitHub پروجیکٹ تیار کریں",
    "priority": "high",
    "completed": false,
    "created_at": "2024-01-15 10:30:45",
    "completed_at": null
  }
]
```

## Features in Detail

### Priority Levels
- 🔴 **High** - فوری کام
- 🟡 **Medium** - عام کام
- 🟢 **Low** - کم اہم

### Statistics Tracked
- 📌 کل کام
- ✅ مکمل شدہ
- ⭕ زیرِ التوا
- 🔴 اہم ترین
- 📈 مکمل شدہ شرح

## Example Usage

```bash
🎯 ٹو-ڈو لسٹ - کمانڈز:
1. add - نیا کام شامل کریں
2. list - تمام کام دیکھیں
3. complete - کام مکمل کریں
...

💭 کمانڈ منتخب کریں: add
📌 کام کا نام: پاکستان کا ٹور
📝 تفصیل (اختیاری): اسلام آباد اور لاہور جانا ہے
⭐ ترجیح (low/medium/high): high
✅ 'پاکستان کا ٹور' شامل کیا گیا (ID: 1)
```

## Technical Details

- **Language:** Python 3.7+
- **Storage:** JSON file
- **Encoding:** UTF-8 (Urdu support)
- **Dependencies:** None (built-in libraries only)

## License

MIT
