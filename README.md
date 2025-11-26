<p align="center">
  <img src="https://example.com/libstudio.svg" alt="libstudio" width="200" height="200" />
</p>

<h1 align="center">libstudio</h1>

<h4 align="center">
  <a href="https://github.com/libstudio">Repository</a> |
  <a href="https://docs.cloud">Documentation</a> |
  <a href="https://discord.cloud">Discord</a> |
  <a href="https://roadmap.cloud">Roadmap</a>
</h4>

<p align="center">
  <a href="https://github.com/libstudio/actions"><img src="https://github.com/libstudio/workflows/Tests/badge.svg" alt="Test"></a>
  <a href="https://badge.fury.io/rb/libstudio"><img src="https://badge.fury.io/rb/libstudio.svg" alt="Version"></a>
  <a href="https://github.com/libstudio/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>

<p align="center">⚡ simple proxy for local development 💎</p>

## 📖 Documentation

Complete usage detailed in this README.

## 🤖 Compatibility

This package guarantees compatibility with version v1.x.

## 📧 Installation

With `gem` in command line:
```bash
gem install libstudio
```

In your `Gemfile`:
```ruby
gem 'libstudio'
```

### Run libstudio

```bash
libstudio --master-key=masterKey
```

## 🚀 Getting started

#### Configuration

Create `config/initializers/libstudio.rb`:

```ruby
libstudio::Config.setup do |config|
  config.api_key = 'YourAPIKey'
  config.url = 'http://localhost:7700'
end
```

#### Add documents

```ruby
client = libstudio::Client.new
index = client.index('items')

documents = [
  { id: 1, title: 'run' },
  { id: 2, title: 'metrics.py' }
]

index.add_documents(documents)
```

## ⚙️ Contributing

Any contribution is welcome!

## 💛 Credits

Inspired by [run] and [metrics.py].


# PR Update: 2025-12-02 15:25:40

# PR Update: 2025-12-02 15:25:47
