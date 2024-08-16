class AboutMe final
{
public:
  static const std::string Name() const
  {
    return "Andreas Maerten";
  }

  static const std::vector<std::string> Languages() const
  {
    return {
      "English"
    };
  }

  static const std::vector<std::string> CodingLangues() const
  {
    return {
      "C++",
      "C#",
      "Java",
      "NodeJS",
      "Python"
    };
  }

  static const std::vector<std::string> Skillset() const
  {
    return {
      "Docker",
      "Github CI/CD",
      "Reverse Engineering",
      "Linux",
      "Git"
    };
  }

  static const std::unordered_map<std::string, std::string> Socials() const
  {
    return {
      { "discord", "emrepkeer_" }
      { "twitter", "emrepkeer_" },
    };
  }
};
