def audcma_v2(multiplicand: int, multiplier: int) -> int:
    """
    Ahmet Ulucay Drag-and-Carry Multiplication Algorithm v2
    - Convolutional Form with right-to-left carry propagation.
    - Preserves the leftmost digit in full.
    """
    # Step 1: Convert numbers to digit arrays
    n_digits = list(map(int, str(multiplicand)))
    m_digits = list(map(int, str(multiplier)))

    # Step 2: Reverse multiplier digits for convolution
    m_digits.reverse()
    k = len(m_digits)

    # Step 3: Pad multiplicand with k-1 zeros on both sides
    padding = [0] * (k - 1)
    padded_n = padding + n_digits + padding

    # Step 4: Slide window of size k and compute dot-products
    dot_products = []
    for i in range(len(padded_n) - k + 1):
        window = padded_n[i:i+k]
        dot = sum(window[j] * m_digits[j] for j in range(k))
        dot_products.append(dot)

    # Step 5: Apply drag-and-carry right to left
    for i in range(len(dot_products) - 1, 0, -1):
        carry = dot_products[i] // 10
        dot_products[i] %= 10
        dot_products[i - 1] += carry

    # Step 6: Convert final digit array to integer
    result_str = ''.join(map(str, dot_products))
    return int(result_str)


# Example
if __name__ == "__main__":
    print("AUD&CMA v2 Result for 5425 × 2431:", audcma_v2(5425, 2431))
