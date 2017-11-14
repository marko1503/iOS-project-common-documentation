// MARK: - UITableView DataSouce
    override func tableView(_ tableView: UITableView, cellForRowAt indexPath: IndexPath) -> UITableViewCell {
        guard let cell = tableView.dequeueReusableCell(withIdentifier: kProductCellIndentifier, for: indexPath) as? PromoProductTableViewCell else { fatalError("Unexpected Cell type") }

        guard let product = self.item(at: indexPath) as? RZProduct else { fatalError("Unexpected item type") }

        return cell
    }
