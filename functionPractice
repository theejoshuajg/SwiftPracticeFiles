import SwiftUI

// Function to find the sum of an array of integers
func findSum(of array: [Int]) -> Int {
    var sum = 0
    for number in array {
        sum += number
    }
    return sum
}

// Function to find the average of an array of integers
func findAverage(of array: [Int]) -> Double {
    guard !array.isEmpty else { return 0 }
    let sum = findSum(of: array)
    return Double(sum) / Double(array.count)
}

// Example SwiftUI view that uses @State
struct ContentView: View {
    @State private var count: Int = 0
    
    var body: some View {
        VStack {
            Text("Counter: \(count)")
                .padding()
            
            Button("Increment") {
                self.count += 1
            }
            .padding()
        }
    }
}

let numbers = [1, 2, 3, 4, 5]
let sum = findSum(of: numbers)
let average = findAverage(of: numbers)
print("Sum:", sum)
print("Average:", average)
