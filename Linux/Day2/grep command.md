# Grep Command in Linux

## 1. Grep म्हणजे काय?

`grep` वापरून आपण एखाद्या file मध्ये विशिष्ट शब्द, अक्षर किंवा pattern शोधू शकतो.

**उदाहरण:**

```bash
grep "ERROR" apps.log
```

## 2. महत्त्वाचे Grep Options

| Command | उपयोग |
|---|---|
| `grep "ERROR" apps.log` | ERROR शोधतो |
| `grep -i "error" apps.log` | मोठे-छोटे अक्षर दुर्लक्षित करतो |
| `grep -n "ERROR" apps.log` | Line number दाखवतो |
| `grep -c "ERROR" apps.log` | किती matching lines आहेत ते मोजतो |
| `grep -v "ERROR" apps.log` | ERROR नसलेल्या lines दाखवतो |
| `grep -w "ERROR" apps.log` | पूर्ण शब्द शोधतो |
| `grep -r "ERROR" .` | Folder मधील files मध्ये शोधतो |
| `grep -l "ERROR" *.log` | ज्या files मध्ये ERROR आहे त्यांची नावे दाखवतो |

## 3. Practical Examples

### Practical 1: ERROR शोधा

```bash
grep "ERROR" apps.log
```

### Practical 2: ERROR किती आहेत ते मोजा

```bash
grep -c "ERROR" apps.log
```

### Practical 3: Line number सोबत ERROR शोधा

```bash
grep -n "ERROR" apps.log
```

### Practical 4: ERROR आणि WARNING दोन्ही शोधा

```bash
grep -E "ERROR|WARNING" apps.log
```

---

**Author:** Linux-AWS-DevOps Practice

**Topic:** Linux Commands – Day 2
