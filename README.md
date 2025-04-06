# Concurrent Email Processor in Go

Demonstrates how to use **goroutines**, **channels**, and **WaitGroups** in Go by simulating a background system that processes incoming emails concurrently.

## How It Works

- A list of email IDs is sent into a `jobs` channel.
- Multiple **worker goroutines** receive jobs, simulate processing, and send confirmation messages into a `confirmations` channel.
- A **collector goroutine** receives and prints the confirmations.
- A `sync.WaitGroup` ensures all processing is completed before the program exits.

## Technologies

- Go (Golang)
- Goroutines
- Channels
- sync.WaitGroup
