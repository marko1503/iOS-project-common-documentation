```swift
// MARK: - UITableView DataSouce
    override func tableView(_ tableView: UITableView, cellForRowAt indexPath: IndexPath) -> UITableViewCell {
        guard let cell = tableView.dequeueReusableCell(withIdentifier: "cellIdentifier", for: indexPath) as? CustomTableViewCell else { fatalError("Unexpected Cell type") }

        cell.textLabel.text = "Custom text"

        return cell
    }
```
